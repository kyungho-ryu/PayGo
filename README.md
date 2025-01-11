# **payGo: Incentive-Comparable Payment Routing Based on Contract Theory**

PayGo is an innovative routing protocol for **Payment Channel Networks (PCN)** that applies **contract theory** to optimize incentives and performance. It addresses the limitations of existing PCN routing protocols by introducing a mechanism to ensure low latency, high throughput, and fair incentives for Payment Service Providers (PSPs).  

## **Key Features**
- **Incentive Mechanism**: Leverages contract theory to derive optimal incentives for PSPs.  
- **Latency and Throughput Guarantees**: Ensures payment latency and throughput with a penalty-based smart contract mechanism.  
- **Blockchain Integration**: Implements the protocol by extending the **Raiden Network**, an Ethereum-based payment channel network.  

For detailed insights, refer to the published paper:  
[**IEEE Access: PayGo - Incentive-Comparable Payment Routing Based on Contract Theory**](https://ieeexplore.ieee.org/abstract/document/9057681)

---

## **Repository Contents**

This repository provides an implementation of the **PayGo protocol** and includes simulations for a P2P topology.  

### **Files and Descriptions**
| **File**               | **Description**                                                                 |
|------------------------|-------------------------------------------------------------------------------|  
| `algorithm.py`         | Implements the incentive mechanism using contract theory.                     |  
| `contract.py`          | Interconnects with the blockchain network.                                    |  
| `key.py`               | Manages blockchain accounts for nodes.                                       |  
| `channelState.py`      | Tracks the state of two nodes participating in the payment channel.            |  
| `message.py`           | Defines the structure of PayGo protocol messages.                             |  
| `node.py`              | Implements the PayGo routing protocol logic.                                  |  
| `settingParameter.py`  | Contains parameters for simulation configuration.                              |  
| `structure.py`         | Manages simulation results and pending payment structures.                    |  

---

## **System Overview**
The PayGo protocol introduces an incentive-compatible routing mechanism by combining:  
1. **Contract Creation**: Each PSP generates a contract bundle, ensuring optimal rewards for latency and throughput.  
2. **Smart Contract Enforcement**: Penalty clauses are enforced through Ethereum-based smart contracts.  
3. **Simulation Environment**: Implements and evaluates the protocol in a P2P topology.  

Below is a high-level overview of the system architecture:

<img src="https://user-images.githubusercontent.com/35050199/78328119-572a2200-75b9-11ea-8060-431963dd0821.png" width="40%"></img>

---

## **How to Run the Project**

### **1. Prerequisites**
- Python 3.x installed.  
- Access to an Ethereum-based blockchain environment (e.g., Ganache).  
- Dependencies listed in `requirements.txt`.

### **2. Setup Instructions**
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-repo-link.git
   cd payGo```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Run the simulation:
```
bash
python simulation.py
```
