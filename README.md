# Udacity Blockchain Capstone

The capstone will build upon the knowledge you have gained in the course in order to build a decentralized housing product.

# Project Resources

- [Remix - Solidity IDE](https://remix.ethereum.org/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Truffle Framework](https://truffleframework.com/)
- [Ganache - One Click Blockchain](https://truffleframework.com/ganache)
- [Open Zeppelin ](https://openzeppelin.org/)
- [Interactive zero knowledge 3-colorability demonstration](http://web.mit.edu/~ezyang/Public/graph/svg.html)
- [Docker](https://docs.docker.com/install/)
- [ZoKrates](https://github.com/Zokrates/ZoKrates)

# Project submission data

Run the tests: truffle test or npm test

https://testnets.opensea.io/collection/havefunusingsolidity-ronlynmxis

Verifier: 0x47bb83076D7fa188b437931793a0EB9A1C06e179
SolnSquareVerifier: 0x1FC63A7c0C8361fE838c10a78EEfCfB9B06fabd3

abi: [
{
"inputs": [
{
"internalType": "address",
"name": "verifier",
"type": "address"
}
],
"payable": false,
"stateMutability": "nonpayable",
"type": "constructor"
},
{
"anonymous": false,
"inputs": [
{
"indexed": true,
"internalType": "address",
"name": "owner",
"type": "address"
},
{
"indexed": true,
"internalType": "address",
"name": "approved",
"type": "address"
},
{
"indexed": true,
"internalType": "uint256",
"name": "tokenId",
"type": "uint256"
}
],
"name": "Approval",
"type": "event"
},
{
"anonymous": false,
"inputs": [
{
"indexed": true,
"internalType": "address",
"name": "owner",
"type": "address"
},
{
"indexed": true,
"internalType": "address",
"name": "operator",
"type": "address"
},
{
"indexed": false,
"internalType": "bool",
"name": "approved",
"type": "bool"
}
],
"name": "ApprovalForAll",
"type": "event"
},
{
"anonymous": false,
"inputs": [
{
"indexed": false,
"internalType": "address",
"name": "caller",
"type": "address"
}
],
"name": "Paused",
"type": "event"
},
{
"anonymous": false,
"inputs": [
{
"indexed": false,
"internalType": "uint256",
"name": "index",
"type": "uint256"
},
{
"indexed": false,
"internalType": "address",
"name": "account",
"type": "address"
}
],
"name": "SolutionSubmitted",
"type": "event"
},
{
"anonymous": false,
"inputs": [
{
"indexed": true,
"internalType": "address",
"name": "from",
"type": "address"
},
{
"indexed": true,
"internalType": "address",
"name": "to",
"type": "address"
},
{
"indexed": true,
"internalType": "uint256",
"name": "tokenId",
"type": "uint256"
}
],
"name": "Transfer",
"type": "event"
},
{
"anonymous": false,
"inputs": [
{
"indexed": false,
"internalType": "address",
"name": "caller",
"type": "address"
}
],
"name": "Unpaused",
"type": "event"
},
{
"anonymous": false,
"inputs": [
{
"indexed": false,
"internalType": "address",
"name": "_owner",
"type": "address"
}
],
"name": "ownerShip",
"type": "event"
},
{
"constant": false,
"inputs": [
{
"internalType": "bytes32",
"name": "_myid",
"type": "bytes32"
},
{
"internalType": "string",
"name": "_result",
"type": "string"
}
],
"name": "**callback",
"outputs": [],
"payable": false,
"stateMutability": "nonpayable",
"type": "function"
},
{
"constant": false,
"inputs": [
{
"internalType": "bytes32",
"name": "_myid",
"type": "bytes32"
},
{
"internalType": "string",
"name": "_result",
"type": "string"
},
{
"internalType": "bytes",
"name": "_proof",
"type": "bytes"
}
],
"name": "**callback",
"outputs": [],
"payable": false,
"stateMutability": "nonpayable",
"type": "function"
},
{
"constant": false,
"inputs": [
{
"internalType": "address",
"name": "to",
"type": "address"
},
{
"internalType": "uint256",
"name": "tokenId",
"type": "uint256"
}
],
"name": "approve",
"outputs": [],
"payable": false,
"stateMutability": "nonpayable",
"type": "function"
},
{
"constant": true,
"inputs": [
{
"internalType": "address",
"name": "owner",
"type": "address"
}
],
"name": "balanceOf",
"outputs": [
{
"internalType": "uint256",
"name": "",
"type": "uint256"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
},
{
"constant": true,
"inputs": [],
"name": "baseTokenURI",
"outputs": [
{
"internalType": "string",
"name": "",
"type": "string"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
},
{
"constant": true,
"inputs": [
{
"internalType": "uint256",
"name": "tokenId",
"type": "uint256"
}
],
"name": "getApproved",
"outputs": [
{
"internalType": "address",
"name": "",
"type": "address"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
},
{
"constant": true,
"inputs": [
{
"internalType": "address",
"name": "owner",
"type": "address"
},
{
"internalType": "address",
"name": "operator",
"type": "address"
}
],
"name": "isApprovedForAll",
"outputs": [
{
"internalType": "bool",
"name": "",
"type": "bool"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
},
{
"constant": false,
"inputs": [
{
"internalType": "address",
"name": "to",
"type": "address"
},
{
"internalType": "uint256",
"name": "tokenId",
"type": "uint256"
}
],
"name": "mint",
"outputs": [
{
"internalType": "bool",
"name": "",
"type": "bool"
}
],
"payable": false,
"stateMutability": "nonpayable",
"type": "function"
},
{
"constant": true,
"inputs": [],
"name": "name",
"outputs": [
{
"internalType": "string",
"name": "",
"type": "string"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
},
{
"constant": true,
"inputs": [],
"name": "owner",
"outputs": [
{
"internalType": "address",
"name": "",
"type": "address"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
},
{
"constant": true,
"inputs": [
{
"internalType": "uint256",
"name": "tokenId",
"type": "uint256"
}
],
"name": "ownerOf",
"outputs": [
{
"internalType": "address",
"name": "",
"type": "address"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
},
{
"constant": false,
"inputs": [
{
"internalType": "address",
"name": "from",
"type": "address"
},
{
"internalType": "address",
"name": "to",
"type": "address"
},
{
"internalType": "uint256",
"name": "tokenId",
"type": "uint256"
}
],
"name": "safeTransferFrom",
"outputs": [],
"payable": false,
"stateMutability": "nonpayable",
"type": "function"
},
{
"constant": false,
"inputs": [
{
"internalType": "address",
"name": "from",
"type": "address"
},
{
"internalType": "address",
"name": "to",
"type": "address"
},
{
"internalType": "uint256",
"name": "tokenId",
"type": "uint256"
},
{
"internalType": "bytes",
"name": "_data",
"type": "bytes"
}
],
"name": "safeTransferFrom",
"outputs": [],
"payable": false,
"stateMutability": "nonpayable",
"type": "function"
},
{
"constant": false,
"inputs": [
{
"internalType": "address",
"name": "to",
"type": "address"
},
{
"internalType": "bool",
"name": "approved",
"type": "bool"
}
],
"name": "setApprovalForAll",
"outputs": [],
"payable": false,
"stateMutability": "nonpayable",
"type": "function"
},
{
"constant": false,
"inputs": [
{
"internalType": "bool",
"name": "status",
"type": "bool"
}
],
"name": "setPausedStatus",
"outputs": [],
"payable": false,
"stateMutability": "nonpayable",
"type": "function"
},
{
"constant": true,
"inputs": [
{
"internalType": "bytes4",
"name": "interfaceId",
"type": "bytes4"
}
],
"name": "supportsInterface",
"outputs": [
{
"internalType": "bool",
"name": "",
"type": "bool"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
},
{
"constant": true,
"inputs": [],
"name": "symbol",
"outputs": [
{
"internalType": "string",
"name": "",
"type": "string"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
},
{
"constant": true,
"inputs": [
{
"internalType": "uint256",
"name": "index",
"type": "uint256"
}
],
"name": "tokenByIndex",
"outputs": [
{
"internalType": "uint256",
"name": "",
"type": "uint256"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
},
{
"constant": true,
"inputs": [
{
"internalType": "address",
"name": "owner",
"type": "address"
},
{
"internalType": "uint256",
"name": "index",
"type": "uint256"
}
],
"name": "tokenOfOwnerByIndex",
"outputs": [
{
"internalType": "uint256",
"name": "",
"type": "uint256"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
},
{
"constant": true,
"inputs": [
{
"internalType": "uint256",
"name": "tokenId",
"type": "uint256"
}
],
"name": "tokenURI",
"outputs": [
{
"internalType": "string",
"name": "",
"type": "string"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
},
{
"constant": true,
"inputs": [],
"name": "totalSupply",
"outputs": [
{
"internalType": "uint256",
"name": "",
"type": "uint256"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
},
{
"constant": false,
"inputs": [
{
"internalType": "address",
"name": "from",
"type": "address"
},
{
"internalType": "address",
"name": "to",
"type": "address"
},
{
"internalType": "uint256",
"name": "tokenId",
"type": "uint256"
}
],
"name": "transferFrom",
"outputs": [],
"payable": false,
"stateMutability": "nonpayable",
"type": "function"
},
{
"constant": false,
"inputs": [
{
"internalType": "address",
"name": "newOwner",
"type": "address"
}
],
"name": "transferOwnership",
"outputs": [],
"payable": false,
"stateMutability": "nonpayable",
"type": "function"
},
{
"constant": false,
"inputs": [
{
"internalType": "uint256",
"name": "index",
"type": "uint256"
},
{
"internalType": "bytes32",
"name": "key",
"type": "bytes32"
}
],
"name": "addSolution",
"outputs": [],
"payable": false,
"stateMutability": "nonpayable",
"type": "function"
},
{
"constant": false,
"inputs": [
{
"internalType": "address",
"name": "to",
"type": "address"
},
{
"internalType": "uint256",
"name": "tokenId",
"type": "uint256"
},
{
"internalType": "uint256[2]",
"name": "a",
"type": "uint256[2]"
},
{
"internalType": "uint256[2][2]",
"name": "b",
"type": "uint256[2][2]"
},
{
"internalType": "uint256[2]",
"name": "c",
"type": "uint256[2]"
},
{
"internalType": "uint256[2]",
"name": "input",
"type": "uint256[2]"
}
],
"name": "verifyMint",
"outputs": [
{
"internalType": "bool",
"name": "",
"type": "bool"
}
],
"payable": false,
"stateMutability": "nonpayable",
"type": "function"
},
{
"constant": true,
"inputs": [
{
"internalType": "uint256[2]",
"name": "a",
"type": "uint256[2]"
},
{
"internalType": "uint256[2][2]",
"name": "b",
"type": "uint256[2][2]"
},
{
"internalType": "uint256[2]",
"name": "c",
"type": "uint256[2]"
},
{
"internalType": "uint256[2]",
"name": "input",
"type": "uint256[2]"
}
],
"name": "getKey",
"outputs": [
{
"internalType": "bytes32",
"name": "",
"type": "bytes32"
}
],
"payable": false,
"stateMutability": "view",
"type": "function"
}
]
