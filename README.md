Step 1: We install nodejs, npm 
Step 2:
 + Install truffle with cmd: npm install -g truffle
 + Install Ganache: https://trufflesuite.com/ganache/
Step 3: cd folder project
+ Setup file truffle-config with your accout ganache
+ Check your smart contract and script test smart contract
Step 4:
+ run cmd: truffle migrate # Build your token
 => This will run all migrations located within your project's migrations directory. At their simplest, migrations are simply a set of managed deployment scripts
 After run cmd: truffle deploy # switch deploy terminal  
+ run test all API of file deploy
== Example:
+ let accounts = await web3.eth.getAccounts() # to get account test
+ instance.sendCoin(accounts[1], 10, {from: accounts[0]}) # Check feature send token
or:
+ let balance = await instance.getBalance(accounts[0]) # Get balance of account
+ balance.toNumber() # convert balance to number to view
