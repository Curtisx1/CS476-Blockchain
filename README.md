# Mini-Blockchain Project

## How to Run

1. Open a new terminal in the project root folder.  
2. Adjust the **main function** in `blockchain.js` to create new transactions.  

   **Example:**
   ```javascript
   console.log(' Mining block #4 ...');
   demoCoin.addBlock(new Block(4, Date.now().toString(), [
     { from: 'Frank', to: 'Dennis', amount: 201 },
     { from: 'Charlie', to: 'Dee', amount: 120 },
   ]));

**Assignment 1**

Results:

<img width="712" height="1231" alt="Assn1_Screenshot1" src="https://github.com/user-attachments/assets/5830e270-61fa-4513-b07b-c0e08b96ddc4" />
<img width="687" height="874" alt="Assn1_Screenshot2" src="https://github.com/user-attachments/assets/f9ffe788-764f-4262-beed-83f82fbdf3e0" />

Reflection:

Adjusting and adding new features to this mini-blockchain was fairly straightforward and easier than I thought it would be. Before putting this together and running it, I always thought blockchain was extremely complicated. This chain is extremely simple and does not have a lot of functionality but has helped me understand how it works "under the hood". The main thing being hashing. I have heard this term before and understood what it meant. The part I did not fully understand or grasp was proof of work. I know ethereum switched from proof of work to proof of stake. The main talking point was reducing its carbon footprint and reducing the impact on the world due to power demands of proof of work. After messing with this small chain, I now see why. Hashing requires a LOT of processing to mine a block. Adding the nonce really highlights how many attempts to mine a block it takes. Multiple that by thousands of blocks and you get a lot of energy use. 

Confirming the validity of the chain is also a cool concept and makes sense once ran in practice. The correct or accepted hash of a block is created with a lot of different variables (index, timestamp, transactions, previous hash, and nonce). If you change just one of these, even slightly, it changes the hash dramatically and makes finding a "tampered with" block straightforward. Adding the zeros makes hacking or editing the chain and allowing it to continue functioning is almost impossible. You would have to successfully remine all of the blocks, which due to enery/time cost, would not be feasible. Overall I am excited to keep adding to the chain. I think the next big improvement would be adding functionality to add transactions without hard coding them into the main function.
