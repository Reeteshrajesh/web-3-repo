# Smart Contract for Payment Channels over Educhain
* Pull the repository and perform the installation steps. There is no need to do these steps more than once on each computer.
* Do not save any private keys on this repository.
* Enjoy!

## Background

Relying on the notion of the payment channels using educhain, this project implements the concept by incorperating SGX (or any equivalent third party abilities). As a result, allowing usage of payment channels over Ethereum while minimizing gas costs and transaction amounts on the Blockchain.
### For Node
If you wish to re-compile the contract (you don't have to do it, and it's better you don't do it unless you have a good reason):
1. cd ..\educhain
1. node compile.js
1. (verify you see all 3 .json files inside \ethereum\build)
1. node deploy.js
1. Save the addresses you get for the factory and for the SGX simulator.
1. The factory address should be placed in \ethereum\factory.js at line 6.
1. Note: Sometimes when you use node compile.js or deploy you get some weird error. in this
      case - open node.js terminal as administrator from windows search, close the code editor and run the command from the
      terminal you opened. It fixes it.

### For Truffle
1. cd to Truffle/contract directory.
1. In the command line:
    1. Windows- mklink Deposit.sol ..\..\educhain\contracts\Deposit.sol
    1. Linux- sudo ln -s Deposit.sol ../../educhain/contact/Deposit.sol
1. cd ..
1. truffle compile
1. truffle migrate

## Front End interaction:
Wait until the command line tells you that compilation was successful.
1. cd back into root directory (not sure if this is a must).
2. Open chrome (or any other browser with metamask) and enter localhost:3000



## Development

In Development
