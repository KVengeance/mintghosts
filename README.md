# **Mint a Ghost**  
A **React.js** application designed for minting NFTs using **Web3** and **Ethereum Smart Contracts**.

---

## **Features**  
- **NFT Minting** - Users can mint NFTs directly from the app by connecting their wallets.  
- **Dynamic Configuration** - Supports dynamic configuration for contract details, gas limits, and costs.  
- **Real-Time Supply Tracking** - Displays the total minted NFTs out of the maximum supply.  
- **Responsive Design** - Fully responsive and styled using **Styled Components**.  
- **Blockchain Integration** - Supports blockchain interaction through **Redux** for state management.  

---

## **Installation**  

### **1. Clone the Repository:**  
```bash
git clone https://github.com/KarolynW/MintAGhost.git
cd MintAGhost
```

### **2. Install Dependencies:**  
```bash
npm install
```

### **3. Setup Configuration:**  
- Edit the configuration file located at:  
  ```
  /public/config/config.json
  ```
- Update contract details, network information, and marketplace links.  

---

## **Usage**  

### **Start the Application:**  
```bash
npm start
```

### **Mint NFTs:**  
1. Connect to your wallet (e.g., **MetaMask**).  
2. Enter the number of NFTs to mint.  
3. Confirm the transaction through your wallet.  
4. View your NFTs on **OpenSea** or your preferred marketplace.  

---

## **Configuration Options:**  
| Key                  | Description                                          |
|----------------------|------------------------------------------------------|
| CONTRACT_ADDRESS     | Smart contract address for the NFT collection.      |
| NETWORK.NAME         | Blockchain network name (e.g., Ethereum Mainnet).    |
| SYMBOL               | NFT collection symbol.                               |
| DISPLAY_COST         | Cost per NFT displayed to the user.                  |
| WEI_COST             | Cost in WEI for blockchain transactions.             |
| GAS_LIMIT            | Gas limit for minting transactions.                  |
| MARKETPLACE          | Marketplace name (e.g., OpenSea).                     |
| MARKETPLACE_LINK     | Link to view NFTs on the marketplace.                 |

---

## **Code Overview:**  

### **App.js**  
- React component managing the UI and user interactions.  
- Implements wallet connection, minting logic, and data fetching from Redux.  

### **Redux Store:**  
- Handles blockchain connection and data retrieval through `blockchainActions` and `dataActions`.  

### **Styled Components:**  
- Provides dynamic and reusable UI components like buttons and containers.  

---

## **Example Flow:**  
1. Connect wallet using the **CONNECT** button.  
2. Select minting amount using **+/-** buttons.  
3. Click **BUY** to mint NFTs.  
4. Transaction progress is displayed, including error handling.  

---

## **Notes:**  
- Ensure the wallet is connected to the correct network specified in the configuration.  
- The gas limit should not be lowered to avoid transaction failures.  
- Test transactions thoroughly on testnets before deployment to the mainnet.  

---

## **License**  
This project is licensed under the **MIT License**.
