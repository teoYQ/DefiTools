# Defi Tools
#####  Autocompounder (Protofi)

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

Do Reach out if you have any questions!