# dapp
Created my own Dapp on localhost due to a version issue with Moralis
![image](https://user-images.githubusercontent.com/60270105/201852509-33fefe24-2fa4-41b7-bba2-a2c7ddb1faf0.png)

Creating a new Dapp in version 2 using NodeJS

# Prerequisites
- Create a Moralis account
- Install and set up your editor of choice (we will use Visual Studio Code [VSC] in this tutorial)
- Install NodeJS
# # Steps
# Create a NodeJS Dapp
Create a new folder for your project
Open the folder in your editor
Initialize a new project via npm

# Set Up an Express Server
Create an index.js file and set up Express with the following code:

const express = require('express')
const app = express()
const port = 3000

app.get('/', (req, res) => {
  res.send('Hello World!')
})

app.listen(port, () => {
  console.log(`Example app listening on port ${port}`)
})
Add a new script to package.json called start:

"scripts": {
  "start": "node index.js"
},
Run the server by calling npm run start.
Make sure that the server runs by going to [<http://localhost:3000>](http://localhost:3000`). It should show "Hello World!".

# Add Moralis to Your Dapp Fetch and Display NFTs with Metadata
Fetch token balances in the getDemoData function:
Now you've created a simple NodeJS server with Express and Moralis that fetches crypto data of the provided address and chain.


