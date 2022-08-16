Commands related to Web3.js

To install web3 - npm install --save web3
To import web3 - let Web3 =require("web3");
To connect with Ganache - let web3 = new Web3(new Web3.providers.HttpProvider("HTTP://127.0.0.1:7545")); [Remember that the ganache must be running]

To get the balance of an account - web3.eth.getBalance("paste the address of the account inside it").then(console.log);

To convert wei into ether - web3.eth.getBalance("paste the address of the account inside it").then(function(result) {console.log(web3.utils.fromWei(result,"ether"));})  

To transfer ether from one account to another - web3.eth.sendTransaction({from:"paste the address of the account inside it",to:"paste the address of the account inside it",value:web3.utils.toWei("1","ether")});4
