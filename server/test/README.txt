export ACTIVE1="74.207.226.87"
export SEED1="45.56.113.232"
export SOLIDITY="173.230.131.117"
export TRUST="50.116.38.222"
export WALLETS="45.33.99.42"
export WITNESS0="45.33.100.235"
export WITNESS1="173.230.132.180"
export WITNESS2="74.207.235.165"


registerwallet 

myfirstwalletpassword
mysecondwalletpassword
mythirdwalletpassword





TBqAawd6wAg8uL413aQezCcWPeradMMnWe
8dee75e5cae2c41a0023cb2d21e7e298132e8eb22983dd34174c13b0e757d5cb

TYMXucFWEJULq5jGYa3fqiUCDZoxTBiZFA
78b56ad97881a19a7c902cae88684f7edbc05dcf1d7814828c543dd4aed9e14f


TWdtsSh3psVGY9jQyUhkmwCX84ArmkHP3p
345401226b1422329e8a0025af1832ca774925b17428b47b27547f7f93e0713d






mkdir FullNode
cd FullNode
git clone https://github.com/tronprotocol/java-tron
cd java-tron
git checkout origin/master
./gradlew build

cp build/libs/java-tron.jar ../
cp src/main/resources/config.conf ../
cd ..

nohup java -jar java-tron.jar -c config.conf&


tail -F logs/tron.log





# trust node for solidity node
# trustNode = "ip:port"
trustNode = "127.0.0.1:50051"
listen.port = 18889








scp ~/.ssh/id_rsa.pub jasonneely@$ACTIVE1:/home/jasonneely/
scp ~/.ssh/id_rsa.pub jasonneely@$SEED1:/home/jasonneely/
scp ~/.ssh/id_rsa.pub jasonneely@$SOLIDITY:/home/jasonneely/
scp ~/.ssh/id_rsa.pub jasonneely@$TRUST:/home/jasonneely/
scp ~/.ssh/id_rsa.pub jasonneely@$WALLETS:/home/jasonneely/
scp ~/.ssh/id_rsa.pub jasonneely@$WITNESS0:/home/jasonneely/
scp ~/.ssh/id_rsa.pub jasonneely@$WITNESS1:/home/jasonneely/
scp ~/.ssh/id_rsa.pub jasonneely@$WITNESS2:/home/jasonneely/








