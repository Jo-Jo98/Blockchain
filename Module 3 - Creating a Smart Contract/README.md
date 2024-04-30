Module 3

Creation of a smart contract using solidity
Tools being used 

- Solidity as a compiler
- Genache - Allow for test enviroment for Ethernet wallet addresses and funding of gas fees


Steps 
- Install Ganache (use the provided files as different versions might not have the same outcome.)
- In the Etherwallet folder, there is a index.html file. Open it and it will take you to and old ethernetwallet site. Only use this site for this exercise.
- Using Solidity as our compiler - make sure you use version 0.4.11 ![Solidity_compiler](<Screenshot 2024-04-30 at 12.28.15.png>)
- Web address for compiler = https://remix.ethereum.org


Outcome
- Once the code is written in Solidity, press compile on the left side of the screen.
- At the bottom of the screen, you will see Bytecode. Copy the bitecode and move over to the EthernetWallet website that was opened when we clicked on the index.html file.
- Click on the top right and select Custom Network - ![custom_node](<Screenshot 2024-04-30 at 12.37.23.png>)
- Open Ganache and make a note of the port number as this will be required in EthernetWallet - ![Genache_port_num](<Screenshot 2024-04-30 at 12.44.07.png>)
- Enter the port number into the EthernetWallet - ![creating_ethernet_wallet](<Screenshot 2024-04-30 at 12.48.00.png>)
- Click on Contracts in the middle of the screen and then Deploy Contract. Copy the bytecode from Solidity and past it in the required field - ![deploying_contract](<Screenshot 2024-04-30 at 12.53.27.png>)
- Go back to Genache and choose any of the addresses and click the key on the right. This will provide you with the private key associated with that wallet. **PLEASE NOTE THAT THIS IS ONLY TRAINING AND YOUR PRIVATE KEYS SHOULD NEVER BE SHARED** Copy the private key and head back to EthernetWallet - ![private_keys](<Screenshot 2024-04-30 at 13.00.40.png>)
- Past your private key in the required field and press unlock - ![unlock_with_PK](<Screenshot 2024-04-30 at 13.04.53.png>)
- Select Sign Transaction and then Deploy Contract. This allows our smart contract to be placed on the ethereum network and will cost some gas fees as  will be shown on the next illustration. ![sign_and_deploy_contract](<Screenshot 2024-04-30 at 13.10.15.png>)
- Back in Ganache, we can see their was a cost of 0.02 ETH to submit the contract - ![contract_cost](<Screenshot 2024-04-30 at 13.11.55.png>)
- First block of the smart contract has been mined which created the contract - ![first_block](<Screenshot 2024-04-30 at 13.12.03.png>)
- Under Transactions, we can find the contract number - ![contract_address](<Screenshot 2024-04-30 at 13.12.11.png>)
- Having the contract address, we can go back to Ethernetwallet but this time click on Interact with our Contract. Enter the contract address in the required field and head over to Solidity again to copy the ABI code. It is at the bottom net to where you copied the bytecode. Once you past it in the required field, click on access underneath. - ![ABI_code](<Screenshot 2024-04-30 at 13.23.23.png>)
- We are now able to interact with the contract as if individuals are buying or selling during an ICO. Examples are as follow:
    - Total StuxCoins Created - ![total_stuxcoins](<Screenshot 2024-04-30 at 13.33.06.png>)
    - Wallet has no StuxCoins - ![StuxCoins_owned](<Screenshot 2024-04-30 at 13.32.41.png>)
    - Purchasing StuxCoins - ![purchase_stuxcoin](<Screenshot 2024-04-30 at 13.33.38.png>)
    - Wallet Equity in StuxCoins - ![stuxcoins_equity](<Screenshot 2024-04-30 at 13.34.19.png>)
    - Equity in USD as 1 StuxCoin = 1 USD - ![Exchange_rate](<Screenshot 2024-04-30 at 13.34.32.png>)
- In Genache, we can follow all the transactions - ![blockchain_transactions](<Screenshot 2024-04-30 at 13.38.25.png>)

Issues
- The code should be refined and tested. At the moment, when running the code, a wallet has the ability to sell more StuxCoins than what they hold in their wallet. 