# ration_blockchain
A simple program to add purchase of the customers in the blockchain.
Follow instructions from the video --> https://youtu.be/auvOpzSDxjs

This repository contains my code following Udemy's Blockchain A-Z™: Learn How To Build Your First Blockchain, by Kirill Eremenko and Hadelin de Ponteves.

## OPERATIONS :

1. Connect Nodes
  - Nodes are running on different port numbers
2. Record transactions in blockchain
  - Each node will add user data : name, uid, address, and purchase
3. Mining blocks
  - Perform proof of work and add transactions to the block
4. Update and validate the copy of the blockchain
  - Check the longest copy of the blockchain
 
## METHODS USED (for sending requests to Postman):

1. connect_node : to connect to other nodes (Post request)

```javascript
{
"nodes": ["http://127.0.0.1:5001",`
"http://127.0.0.1:5002",`
"http://127.0.0.1:5003"]`
}
```

2. get_chain : to get the blockchain copy (Get Request)
3. add_transaction : add user information (Post Request)

```javascript
{
"name": "",
"uid": "",
"address": "",
"purchase": ""
}
```

4. mine_block : perform proof of work, if successful mine the block (Get Request)
5. replace_chain : to find the longest chain in the entire blockchain network (Get Request)
6. is_valid : validate whether the blockchain is valid or not (Get Request)
7. verify all the hash values

## OTHER METHODS
1. create_block : once proof of work is found block will be created
2. get_previous_block : get the index of the previous block
3. proof_of_work : compute the desired hash challenge
4. hash : returns the hash value
5. add_node : for connecting the nodes
