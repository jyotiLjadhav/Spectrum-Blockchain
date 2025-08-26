# Spectrum Blockchain Simulation

## Project Overview

This project simulates a wireless communication environment where **Primary Users (PU)** and **Secondary Users (SU)** interact. SUs use cognitive radio to sense unused spectrum and share data with other SUs using a blockchain for secure, tamper-proof record-keeping.

## Main Components

- **Blockchain Core**
  - `block.py`: Defines a single block in the blockchain.
  - `blockchain.py`: Manages the chain of blocks, mining, and consensus.
  - `transaction.py`: Handles transactions between users.
  - `wallet.py`: Manages user wallets and cryptographic keys.
  - `node.py`: Runs a Flask web server for blockchain operations and exposes REST APIs.

- **Simulation & GUI**
  - `crub.py`: Simulates the wireless environment, node creation, spectrum sensing, and integrates with the blockchain.
  - **Images**: `PU_small.ppm` and `SU_small.ppm` are used for visualizing PUs and SUs in the GUI.

- **Web UI**
  - `UI/node.html`: Web interface for wallet management, transactions, mining, and viewing the blockchain.
  - `UI/network.html`: Web interface for managing peer nodes in the network.

- **Utilities**
  - `utility/hash_util.py`: Provides hashing functions.
  - `utility/printable.py`: For pretty-printing objects.
  - `utility/verification.py`: For verifying transactions and blocks.

## How It Works

1. **Simulation**  
   - Run `crub.py` to simulate PUs and SUs, spectrum sensing, and data sharing.
   - SUs sense available frequencies and use blockchain to record and share spectrum usage.

2. **Blockchain**  
   - Each transaction (e.g., spectrum access) is recorded in a block.
   - Mining adds new blocks to the chain, securing the data.

3. **Web Interface**  
   - Use the web UI to create wallets, send transactions, mine blocks, and view the blockchain.
   - Manage peer nodes for a distributed network.

## Getting Started

1. **Install dependencies**
   - Python 3.12+
   - Flask, Flask-CORS, requests, cryptography, ecdsa, pycryptodome

2. **Run the simulation**
   - Start with `crub.py` or use the Jupyter notebook `ExecuteFolder.ipynb`.

3. **Start the web server**
   - Run `node.py` and open the UI in your browser.

4. **Interact**
   - Create wallets, send transactions, mine blocks, and manage nodes via the web UI.

## Folder Structure

- **Main Python files**: blockchain logic and simulation
- **UI/**: Web interface files
- **utility/**: Helper modules
- **Images**: PU/SU visualization

---

For more details, see the code in `block.py`, `crub.py`, and# Spectrum Blockchain Simulation

## Project Overview

This project simulates a wireless communication environment where **Primary Users (PU)** and **Secondary Users (SU)** interact. SUs use cognitive radio to sense unused spectrum and share data with other SUs using a blockchain for secure, tamper-proof record-keeping.

## Main Components

- **Blockchain Core**
  - `block.py`: Defines a single block in the blockchain.
  - `blockchain.py`: Manages the chain of blocks, mining, and consensus.
  - `transaction.py`: Handles transactions between users.
  - `wallet.py`: Manages user wallets and cryptographic keys.
  - `node.py`: Runs a Flask web server for blockchain operations and exposes REST APIs.

- **Simulation & GUI**
  - `crub.py`: Simulates the wireless environment, node creation, spectrum sensing, and integrates with the blockchain.
  - **Images**: `PU_small.ppm` and `SU_small.ppm` are used for visualizing PUs and SUs in the GUI.

- **Web UI**
  - `UI/node.html`: Web interface for wallet management, transactions, mining, and viewing the blockchain.
  - `UI/network.html`: Web interface for managing peer nodes in the network.

- **Utilities**
  - `utility/hash_util.py`: Provides hashing functions.
  - `utility/printable.py`: For pretty-printing objects.
  - `utility/verification.py`: For verifying transactions and blocks.

## How It Works

1. **Simulation**  
   - Run `crub.py` to simulate PUs and SUs, spectrum sensing, and data sharing.
   - SUs sense available frequencies and use blockchain to record and share spectrum usage.

2. **Blockchain**  
   - Each transaction (e.g., spectrum access) is recorded in a block.
   - Mining adds new blocks to the chain, securing the data.

3. **Web Interface**  
   - Use the web UI to create wallets, send transactions, mine blocks, and view the blockchain.
   - Manage peer nodes for a distributed network.

## Getting Started

1. **Install dependencies**
   - Python 3.12+
   - Flask, Flask-CORS, requests, cryptography, ecdsa, pycryptodome

2. **Run the simulation**
   - Start with `crub.py` or use the Jupyter notebook `ExecuteFolder.ipynb`.

3. **Start the web server**
   - Run `node.py` and open the UI in your browser.

4. **Interact**
   - Create wallets, send transactions, mine blocks, and manage nodes via the web UI.

## Folder Structure

- **Main Python files**: blockchain logic and simulation
- **UI/**: Web interface files
- **utility/**: Helper modules
- **Images**: PU/SU visualization

---

For more details, see the code in `block.py`, `crub.py`, and