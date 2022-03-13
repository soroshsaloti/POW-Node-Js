# Proof of work blockchain network 
- Node Js
- Docker
- Java Script

# Node Componnent
- express
- body-parser
- uuid
- request-promise

# Start Package
Project startby npm run and [node_1,node_2,node_3,node_4,node_5,node_6]

## Call API
Network API includes 10 actions that description on the bove 

### blockchain
this method action for call first and method is get so you can see all transaction and block create.

### transaction
this method action for create transactin and the method use **POST** with **JSON** body.
>`{
    "amount": 100,
    "sender": "NNFANSDFHYHTN90A09SNFAS",
    "recipient": "IUW099N0A90WENNU234UFAW"
}`

### transaction broadcast
this method action for creating transaction and broadcast to all network nodes.the method use **POST** with **JSON** body.
>`{
    "amount": 100,
    "sender": "NNFANSDFHYHTN90A09SNFAS",
    "recipient": "IUW099N0A90WENNU234UFAW"
}`

### mine
this method action for calculating block to all network nodes.the method use **GET** without any parameter.

### receive-new-block
this method action for receiving a new block in the node. the method use **POST** and called by mine per node.

### register-and-broadcast-node
this method action for registering a new network in the node the broad cast to all valid network. the method use **POST**.

### consensus
the consensus protocol makes sure that every **new block** that is added to the **Blockchain** is the one and only version of the truth that is agreed upon by all the nodes in the Blockchain. the method use **GET**.

### block/:blockHash
Search **a block** by **block hash**. the method use **Get**.This method for **blockchain Explorer**.

### transaction/:transactionId
Search **a block** by **transaction Id** block. the method use **Get**.This method for **blockchain Explorer**.

### address/:address
Search **a block** by **address** block. the method use **Get**.This method for **blockchain Explorer**.
