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
