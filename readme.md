CS765: Introduction of Blockchains, Cryptocurrencies, and Smart Contracts 

Project part 1: Simulation of a P2P Cryptocurrency Network

Group Members:
Niteen Pawar (22M0800)
Darshit Gandhi (22M0824)
Abhijeet Singh (22M0749)


Compiling and running the code :
1. python3 main.py <Number of nodes> <Ttx (TXN Interarrival mean time)> <percent of slow nodes> <percent of low CPU nodes>

2. The program will run for 30 sec. After the code runs successfully, the blockchain tree for each node will be displayed and will be saved in a png file. Also, the longest chain for each node will be displayed and will be saved in a png file.

3. Also, a txt file will be created for each node which contains the block ids and its corresponding arrival time of each block present in that node's blockchain tree.


Files:
1. main.py: This file will take the required command line inputs. Then it will create a randomly connected graph between 4 and 8 other peers from n nodes by taking help from generate_graph.py. Then, it will initiate the initial TXN and initial block generation event. It will then pop events one by one from the events queue, and based on the event type, it will do the processing. There will be 4 types of events: TXN_GEN, TXN_REC, BLK_GEN, and BLK_REC. Then, after all the processing, it will display the blockchain tree and longest chain for each node.

2. node.py: This file contains various properties and data structures required by the node. This also includes functions for TXN Generation, TXN Receive, BLK Generation and BLK Receive.

3. generate_graph.py: It will create a randomly connected graph to between 4 and 8 other peers from n nodes

4. transaction_object.py: This file contains the parameters required for a transaction object.

5. block.py:  This file contains the parameters required for a block object.

6. event.py: This file contains the parameters required for an Event object.

7. global_data.py: This file contains the global parameters that can be required by many other files.




CS765: Introduction of Blockchains, Cryptocurrencies, and Smart Contracts 

Project part 2: Simulating a selfish mining attack and Stubborn Mining attack using the P2P Cryptocurrency Network.
Group Members:
Niteen Pawar (22M0800)
Darshit Gandhi (22M0824)
Abhijeet Singh (22M0749)

1. Compiling and running the code :

python3 main.py n Ttx z0 z1 hp zeta
n = Number of nodes
Ttx = TXN Interarrival mean time
z0 = percent of slow nodes
z1 = percent of low CPU nodes
alpha = Hashing Power of the attacker
zeta = The fraction of honest nodes, an adversary is connected to


2. The program will run until a particular amount of blocks are created. After the code runs successfully, the blockchain tree for each node will be saved in a png file. Also, the longest chain for each node will be saved in a png file.

3. Also, a txt file will be created for each node which contains the block ids and its corresponding arrival time of each block present in that node's blockchain tree.


Files:
1. main.py: This file will take the required command line inputs. Then it will create a randomly connected graph between 4 and 8 other peers from n nodes by taking help from generate_graph.py. Then, it will initiate the initial TXN and initial block generation event. It will then pop events one by one from the events queue, and based on the event type, it will do the processing. There will be 4 types of events: TXN_GEN, TXN_REC, BLK_GEN, and BLK_REC. Now, the selfish mining attack and the stubborn mining attack will be executed based on the hashing power and zeta. Then, after all the processing, it will display the blockchain tree and longest chain for each node.

2. node.py: This file contains various properties and data structures required by the node. This also includes functions for TXN Generation, TXN Receive, BLK Generation and BLK Receive. Also, Node.py contains the code to perform the Selfish mining attack and the Stubborn Mining attack.

3. generate_graph.py: It will create a randomly connected graph to between 4 and 8 other peers from n nodes

4. transaction_object.py: This file contains the parameters required for a transaction object.

5. block.py:  This file contains the parameters required for a block object.

6. event.py: This file contains the parameters required for an Event object.

7. global_data.py: This file contains the global parameters that can be required by many other files.

