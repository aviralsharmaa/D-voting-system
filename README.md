
# Blockchain Decentralized Voting System

### A vote’s Story

A user will walk into a government center and complete his/her biometric verification. Once the verification is complete the user will be taken to web-based portal (developed by our team) where he/she shall be presented with the voting options. The portal then sends the information of the user’s vote encrypted to backend (developed by our team) where the data will be decrypted and the vote’s transaction from the user to the candidate will take place using Ganache blockchain software service. The candidate with the most vote is elected. During each election time the users are that are voted are logged which will make sure only one transaction can be made by user during the whole election process.

### TOOL AND TECHNIQUES USED FOR THE PROJECT

•	HTML

•	CSS

•	JS

•	Solidity

•	Metamask

•	Ganache

•	Truffle


## Installation
#### Compile Smart Contract:

1.	The smart contract is made by Solidity Programing languages. It is a tool that which a blockchain can be deployed in backend of the website,
This smart contract made by our team 
 
2.	To compile smart contract, we use truffle to check the smart contract correctly compiled and check for the error in the smart contract.

3.	Use this command in terminal dashboard in VS code

    `truffle compile`
    
    ![1](https://user-images.githubusercontent.com/71272614/226087969-1b86485f-cf3c-4189-b57d-eb202b890a7c.png)

4.	It will compile the smart contract.
  	
#### Deploy Smart contract

5.	`truffle migrate –reset`

![2](https://user-images.githubusercontent.com/71272614/226087985-deb3c0d0-cf95-43a0-99a3-ee53f19a0f19.png)


6. Smart contract will deploy on the blockchain. Which is in our local host.

![3](https://user-images.githubusercontent.com/71272614/226088001-a5f11e8f-5036-4ba5-a57a-58538c95e642.png)


7.	Open Ganache, it is a software which gives 10 accounts, with balance of 100 ethereum i.e., on our local system. Which is not a real Ethereum coins.

8.	Type on terminal `truffle console`
![4](https://user-images.githubusercontent.com/71272614/226088009-9509b57c-f2e1-49ac-8945-7629ce81d9f1.png)


9.	Type `election = await Election.deployed()`

![5](https://user-images.githubusercontent.com/71272614/226088020-e4ad8f90-0cd0-4a7c-bad5-8842ed82484f.png)


10.	Type ``election``

![6](https://user-images.githubusercontent.com/71272614/226088025-7b7c344d-9bc0-43e2-9f08-7fa2a07af15d.png)


11.	Our aim is to find the address to communicate with smart contract.

12.	Type ``election.address``

![7](https://user-images.githubusercontent.com/71272614/226088038-92c4faf2-5383-43b0-b9f8-d56a8fe12cd6.png)


13.	It will show us the address of a blockchain that will be deployed on our smart contract.

14.	 Copy that address and pate it to the 
`Clint/src/components/Result.js`\
`Clint/src/components/VotingArea.js`
	
15.	 Now copy the file of election in which your workspace is saved in;
`build/contracts/Election.json`

16.	 Paste and replace that file in;
`Clint/src/abi`

#### Copy the address (Unique Identity)
	
17.	 Copy the address of the ganache 10 account and paste it in;
`Client/src/data.json`\
`Server/index.js`

### To run server

#### Run two terminal simultaneously

18.	 Jump to the directory in server;

`Cd/server`\
`Nodemon index.js`


19.	 Jump to the directory in client;

  `Cd/client`\
  `npm start `


### RESULTS (SCREENSHOTS)

![login1](https://user-images.githubusercontent.com/71272614/226088061-ab5e6195-b34c-4cd4-b160-cc60d67af5c7.png)

![login2](https://user-images.githubusercontent.com/71272614/226088067-885c40d3-4d4b-4836-9d2f-f9a5d673a389.png)

![login3](https://user-images.githubusercontent.com/71272614/226088069-80286d66-6bf6-41c6-b629-865bb8e5bcfe.png)

![login4](https://user-images.githubusercontent.com/71272614/226088073-63e70c42-2c80-44d3-910a-bcd98405ab8a.png)

![login5](https://user-images.githubusercontent.com/71272614/226088076-56f1b039-2925-4b72-90d1-c3ffbdd0e28b.png)


    
