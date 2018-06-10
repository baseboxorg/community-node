




https://github.com/tronprotocol/Documentation/blob/master/TRON_Protocol/Transition_Manual_for_Exchanges_and_TRX_EN.md.  

**STEP 4 Install Command Line Wallet**

Technically the wallet doesn't work yet, but we're one step closer with this latest build. Unless you installed screen as per the Google Cloud video, you'll need to open a second terminal window to work while the java-tron is running.

    git clone https://github.com/tronprotocol/wallet-cli.git
    cd wallet-cli
    ./gradlew build       
    cp src/main/resources/config.conf .
	nano config.conf
Point your wallet-cli to the new witness node if you want by changing the first block of the wallet-cli/config.conf file

	fullnode = {
	  ip.list = [
	    "12.34.56.78:50051"
	  ]
	}
12.34.56.78 is just an example. Use your IP address of the java-tron witness node. N.B. even though the server may be running on port 18888 you should set this port to 50051. This is the proper location for the config file and it's one less error generated when your start up.

    ./gradlew run -Pcmd
After it gets to 90% you will have an active cursor. 

At this point it's a bit of a best guess, since the test net isn't fully connected. When I run the blockchain explorer I don't see any nodes or any blocks, so it's not surprising that the login doesn't work. Even still, I'm not 100% sure how it's supposed to work. I believe you ought to be able to just login with the password you got when you registered at tronscan.org 

    login YOUR_PASSWORD_HERE
But that has yet to work for me. It shouldn't need a network connection to login. The address is generated from the password when the wallet was originally registered. TRON Docs say this about the RegisterWallet Command:

> *RegisterWallet* Register a wallet in local. Generate a pair of ecc keys. Derive a AES Key by password and then use the AES algorithm to encrypt and save the private key. The account address is calculated by the public key sha3-256, and taking the last 20 bytes. All subsequent operations that require the use of a private key must enter the password.

I kind of got lost in this explanation but does this mean the password will generate a different address on every machine running the wallet? Because that's the behavior right now. That can't be right. You have to be able to print up this stuff to make a cold wallet transferable to any computer. If all I have is my password, address and my private key printed out and my wallet gets destroyed I should be able to use that password to log in with a different wallet and still be connected to the same address.

TRON devs posted an update:

> "The way addresses are generated changed a few times and it is gonna be changed (again) to base58 format soon."

That explains why my wallet isn't sharing info with the blockchain, but it doesn't explain why two different computers running the same version of the wallet come up with different addresses.

Logically this should be the same address and private key but like the devs said things are changing fast. It doesn't make sense either that you need to register this wallet. But I think once my blockchain explorer can see the nodes and blocks my wallet will be able to log in without the need to register the wallet. It's either that, or the wallet is creating an **actual wallet** for cold storage. 

    RegisterWallet YOUR_PASSWORD_HERE
    login YOUR_PASSWORD_HERE
    getAddress
    BackupWallet YOUR_PASSWORD_HERE
You'll want to back up everything (None of any of this is going to be valid on main.net, but get in the habit). This doesn't actually back anything up, just prints your address and private key that you need to save. Ideally this should be the same as what you saw at tronscan.org. I know that it's not sharing the same information as the rest of the blockchain, because when logged in to Tronscan.org I can send TRX to the address created in wallet-cli, and it says success but my wallet-cli balance doesn't change.

    getbalance
    listAccounts
    listNodes
I usually get about 190 nodes. ListAccounts only shows the ones listed in my java-tron config file, the tronscan.org blockchain explorer shows new ones coming online often.

When the wallet starts up, it knows where to get its blockchain data.  

In the wallet-cli terminal there are a lot of useful commands. Type ? for a list. There's no point in walking you through most of them since we don't have a balance sync'd up. The command everyone wants to use is assetIssue, but unfortunately it's got a bug. If you don't enter 10 elements in the array, it throws an error. But the underlying code is expecting 11 elements before it can create the object. I tried haxoring the code to make it expect 11 elements, but no go. They forgot VoteScore in their example doc.

    AssetIssue Password AssetName TotalSupply TrxNum AssetNum StartDate EndDate DecayRatio VoteScore Description Url

Eventually the command will look like this:

    assetIssue YOUR_PASSWORD_HERE Test1 10000000000000000 1 100 2018-4-1 2018-4-30 1 5 just-test https://github.com/tronprotocol/wallet-cli/

**BLOCKCHAIN EXPLORER**
If you go to https://tronscan.io/ you can access a web wallet.  An identical page has been set up at https://tronscan.org/#/

There are two ways for you to run one. The first is

    cd ~/wallet-cli/build/libs
    java -jar wallet-1.0-SNAPSHOT.jar
then directing your browser to http://serveripaddress:8088

The standalone version of this app is wallet-web. In order to install wallet-web you need Yarn. I needed to upgrade to yarn 1.5.1 because 1.3 didn't work.  Yarn 1.3 is actually a symlink from cmdtest, so this is what my workflow looked like

    sudo apt-get remove cmdtest libuv1
    sudo apt-get remove yarn
    sudo npm install -g yarn
    git clone https://github.com/tronprotocol/wallet-web
    cd wallet-web
    yarn install
    yarn start
then directing your browser to http://serveripaddress:3000
If you try to install wallet-web without the right version of Yarn installed you will bork the install because the installer will already have staged the files incorrectly. To fix this you have to delete the contents of node-modules

    sudo rm -Rf ~/wallet-web/node-modules/*
then run 'yarn install' again

However, when I run the explorer it doesn't show any blocks like the other sites do.
