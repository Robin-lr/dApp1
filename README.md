# LearnWeb3 First dApp - Mood Diary

This is a simple decentralized application (dApp) that allows users to store and retrieve their mood on the Ethereum Sepolia testnet using a smart contract.

## **Features**
- Connects to an Ethereum wallet (such as MetaMask)
- Allows users to set and get their mood on the blockchain
- Interacts with a smart contract deployed on the Sepolia testnet

## **Technologies Used**
- **Frontend:** HTML, JavaScript
- **Ethereum Interaction:** [Viem.js](https://viem.sh/)
- **Blockchain:** Ethereum Sepolia testnet
- **Smart Contract:** Solidity

## **Setup Instructions**
### **Prerequisites**
- A browser with [MetaMask](https://metamask.io/) or another Ethereum wallet installed
- Node.js installed (optional, if you want to run a local development server)

### **Steps to Run Locally**
1. Clone this repository:
   ```sh
   git clone <your-repo-url>
   cd your-repo-name
   ```
2. Open `index.html` in a browser.
3. Connect your wallet when prompted.
4. Enter a mood in the input field and click **Set Mood**.
5. Click **Get Mood** to retrieve the stored mood from the blockchain.

## **Smart Contract**
The smart contract (`MoodDiary.sol`) is deployed on the Sepolia testnet and consists of:
- `setMood(string memory _mood)`: Stores a given mood string on the blockchain.
- `getMood()`: Retrieves the stored mood.

### **Contract Address**
```
0x67085B2E12BB13a7824eB9C65a3dB94C1179e33C
```

## **Potential Issues & Fixes**
1. **Wallet Not Connected**: Ensure MetaMask is installed and connected to Sepolia.
2. **Contract Not Responding**: Check the console for errors and verify that the contract address is correct.
3. **Gas Fees Required**: Since `setMood` is a state-changing transaction, ensure you have Sepolia ETH for gas fees.

## **Security Considerations**
- **Is it safe to make this repo public?**  
  Yes, making this repo public is generally safe. However, avoid committing:
  - Your private keys or seed phrases.
  - Any sensitive user data.

## **License**
This project is open-source under the MIT License.
