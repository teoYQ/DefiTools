# Defi Tools
####  Autocompounder (Protofi)

- Requirements
    - Node (https://nodejs.org/en/download/)
    - Run the following command in terminal (npm install web3) 
    - Metamask Wallet (https://metamask.io/download/)
    - Metamask private key (https://metamask.zendesk.com/hc/en-us/articles/360015289632-How-to-Export-an-Account-Private-Key)
- How to Run
    1) Clone the repository
    2) In line 3 of ProtoCompounder.js, insert ur private key 
        `const wallet = web3.eth.accounts.wallet.add('INSERT YOUR PRIVATE KEY HERE')`
    3)  In line 91 of ProtoCompounder.js set your polling interval ( defualt is at 6hours )
    `const POLLING_INTERVAL = 21600000 // 1000 = 1s , 60000 = 1 min`
    4) Save the file, launch your terminal and run 
    `node ProtoCompounder.js`   

##### Additional info
This works for the nuclues farm $PROTO - $FTM LP and stakes the electrons earned into the fission pool. Everytime electrons are staked in the fission pool, the $DAI farmed is collected as well.<br>
You can easily modify this by changing the farm id to work for $PROTO - $USDT instead in line 15. set `farm id = 2`<br>
The code can be easily modified to make it work for fusion farms, harvest $PROTO, stake in Particle farm. Or if you're more adept at coding, then you could do a harvest $PROTO, sell half of the $PROTO and form a $PROTO - $FTM LP, stake the LP and harvest $ELCT and stake in fission for the maximum APY!<br>
Do Reach out if you have any questions!


####  Tomb & Tombforks autocompounder

- Requirements (Same as above)
    - Node (https://nodejs.org/en/download/)
    - Run the following command in terminal (npm install web3) 
    - Metamask Wallet (https://metamask.io/download/)
    - Metamask private key (https://metamask.zendesk.com/hc/en-us/articles/360015289632-How-to-Export-an-Account-Private-Key)
- How to Run
    1) Clone the repository
    2) In line 3 of TombFork.js, insert ur private key 
        `const wallet = web3.eth.accounts.wallet.add('INSERT YOUR PRIVATE KEY HERE')`
    3)  In line 91 of TombFork.js set your polling interval ( defualt is at 6hours) aka how often to compound
    `const POLLING_INTERVAL = 21600000 // 1000 = 1s , 60000 = 1 min`
    4) Save the file, launch your terminal and run 
    `node TombFork.js`   

##### Additional info
The sample code already works for ScarabFinance and should work for Tomb and most tomb forks ( unless their contracts are not verified, then you cant get the contract ABI. This code automatically harvest $TSHARE from ur tomb-ftm LP (gscarab and scarab-ftm LP respectively for scarabfinance) and deposits it in the Masonry (temple for scarab finance) <br>
You can easily modify this by changing the pid to work for $TSHARE - $FTM instead in line 12. set `pid = 1`<br>
Will be upgrading this automation tool to sell 50% of the $TOMB collected from the masonry into $FTM to form the TOMB - FTM LP and deposit it back into the Cemetry<br>
Do Reach out if you have any questions!