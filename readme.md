
# Readme #

This is the readme for this project , stating all the steps that has been performed in order for succesful execution.

## Install Visual Studio Code ##

```https://code.visualstudio.com/Download```

Once your visual code in install you can download node js from :

## Install NodeJs ##

```https://nodejs.org/en/download/```

## Taking the code from zip folder  ##

Unzip the code folder containing all the files and from command prompt or git bash prompt write code . 
This will open the entire code in visual editor , where you can run or debug the code as per your requirement 

## for the moment ##

you need to run npm install , to install all dependencies from package.json
## Executing the project ##

1. Create a metamask account and copy your profile id.
2. Download Remix and copy ozERC20.sol file to compile and deploy through your custom token to create a contract.
3. Once the contract is created , copt the contract id and save it .
4. Create an account on infura to create an project for your ropsten endpoint and copt the endpoint API.
5. Once above steps are done, create a .env file and mention below vales - 
INFURA_TOKEN = **************
CONTRACT_ADDRESS = **********
OWNER_ADDRESS = ***********
SUPER_SECRET_PRIVATE_KEY = ***************

a working .env file has been provided for mycode execution

## Executing a .JS file ##

To execute a javascript file using node.js, run the following command:

after succesfull installation of all npm dependencies from package.json 
run 
node contract.js
node distribut.js - it will distibute tokens to 10 accounts mentioned in account.txt


## CURL accessing of handlers"

To POST to a route, execute the following CURL command:

```curl -XPOST http://localhost:8080/transfer -H 'content-type: application/json' -d '{"account_to": "0x8B91cD4EE40E267d7C4Ce36D7b8Ff4a0E96E06FD", "amount": "123000"}'```


## Docker ##

crerating a custom docker image for the container to run in background .
### View running docker containers ###

docker --version
docker image ls
docker container ps

### build a docker container ###

docker build -t teenakohli2286/blockchainimage .

### run the image -d for background process###

docker run -p 8080:8080 --name nci -d teenakohli2286/blockchainimage

### view logs ###
to view logs once can use 2 intials of dockerprocess 

docker conatiner logs af

## docker hub image 
created a account on docker and push the image to docker hub.io
docker push -t latest teenakohli2286/blockchainimage
Using default tag: latest
The push refers to repository [docker.io/teenakohli2286/blockchainimage]

and can be oublically accesed - 
https://hub.docker.com/repository/docker/teenakohli2286/blockchainimage


## Requirements for Assignment ##

### 1. create an ethereum account ###
Account id - 0xaD21146De8C91BB1521850028281a47a0426954D
This is completed inside metamask (12 words, create an account, fund with Ropsten ether)

### 2. Create an ERC20-compliant, fixed-supply token
using open zeppelin contract, 
 TrialDeploy.TOK 

### 3. Deply to Ropsten
deploying using injected web3 and metamask
https://ropsten.etherscan.io/token/0x8b91cd4ee40e267d7c4ce36d7b8ff4a0e96e06fd?a=0xaD21146De8C91BB1521850028281a47a0426954D


