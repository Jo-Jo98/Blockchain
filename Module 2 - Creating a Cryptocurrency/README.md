In Module 2 

In this Module, the implementation of running the code on seperate nodes is implemented. This is to simulate the nodes joining the network and confirming the principle of longest chain remain.

Stux 5001, Stuc 5002 & Stux 5003 is all the same code but represent different nodes using different ports within our enviroment. 

We also have 2 json files - node.json is the 3 different nodes as we mentioned and transaction.json is a place holder for transactions that will be carried out on the network. 

StuxCoin.py would be the code distributed to other miners that would want to join the network. 

Once all 3 nodes are running on the network, use POSTMAN to GET the chain, update the chain through POST request and play around with the new network.

1 - Running code on seperate nodes = ![Running Nodes](<Screenshot 2024-04-30 at 11.34.27.png>)
2 - get_chain - ![get_chain_request](<Screenshot 2024-04-30 at 11.35.17.png>)
3 - connect_node - ![connect_node](<Screenshot 2024-04-30 at 11.37.45.png>)
4 - connect_node - ![2nd_node_connect](<Screenshot 2024-04-30 at 11.41.10.png>)
5 - add_transaction - ![adding_transaction](<Screenshot 2024-04-30 at 11.43.52.png>)
6 - mine_block - ![blocks_mined](<Screenshot 2024-04-30 at 11.45.01.png>)
7 - replace_chain - ![longest_chain](<Screenshot 2024-04-30 at 11.54.00.png>)
