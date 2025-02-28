**Griffin Blockchain**

*Overview*

Griffin Blockchain is a blockchain miner written in Java as part of the CSIS 294 course. It demonstrates the fundamental components of blockchain technology, including transaction processing, Merkle tree generation, and proof-of-work mining. Developing this project felt like solving a complex puzzle—one block at a time.

*Features*

- ✅ **Transaction Handling**: Accepts transactions from both user input and remote nodes.
- 🔗 **Peer-to-Peer Communication**: Uses socket programming to send and receive messages between miners.
- ⚡ **Proof-of-Work**: Implements a simple algorithm for mining valid blocks.
- 🌳 **Merkle Tree Generation**: Constructs a Merkle tree from transactions.
- 🔄 **Multi-threading**: Runs the miner and server in separate threads for smooth operation.
- 📩 **Custom Message Queue**: Manages incoming messages with a queue system.

*Project Structure*

| File                 | Description |
|----------------------|-------------|
| `Block.java`        | Defines the block structure and hashing methods. |
| `BlockchainBasics.java` | Main class that starts the miner and P2P server. |
| `BlockchainUtil.java` | Provides SHA-256 hashing and helper methods. |
| `MerkleNode.java`    | Represents a node in the Merkle tree. |
| `Miner.java`        | Handles mining, proof-of-work, and transactions. |
| `P2PMessage.java`   | Defines P2P messages between nodes. |
| `P2PMessageQueue.java` | Implements a queue for P2P messages. |
| `P2PServer.java`    | Manages incoming socket connections. |
| `P2PUtil.java`      | Provides network communication utilities. |

*How to Run*

Compile the Code: Ensure Java is installed, then compile all Java files in the project directory.

Start the Application: Run BlockchainBasics.

Set Up Miner: Enter a miner username and specify a port number for the server.

Choose Mode: When prompted with "Send transactions to another miner (y,n)?", enter n to run a standalone instance for testing.

Enter Transactions: Input transactions when prompted. Once enough transactions (typically 4) are collected, the mining process will start.

Test Networking: To test peer-to-peer features, run another instance of the app on a different port and follow on-screen prompts to establish a connection.

*Testing*

Run the application in an IDE.

Select n when asked about sending transactions to another miner.

Enter transactions until a block is successfully mined.

Capture a screenshot of the final block details as required for documentation.

*Future Work*

Griffin Blockchain started as a basic miner but evolved into a more comprehensive blockchain system in class. Enhancements included proper block chaining, improved network node management, and a simple consensus mechanism. Future development may explore:

Implementing smart contract support.

Enhancing security features.

Optimizing consensus mechanisms.
