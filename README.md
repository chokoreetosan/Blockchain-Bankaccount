# Blockchain-Bankaccount-
Creates a smart contract on the tron blockchain that can store funds which the user can withdraw by providing a password.  This project currently respects no security practices, and is intended to be a teaching tool.  It contains an extremely simple smart contract and an extremely simple node app that utilizes it.

Included is: 
+The original smart contract deployment address.  
+The original smart contract code.
+A simple node app that utilizes the contract.

If you want to to deploy the smart contract on the blockchain, I suggest [tronbox](https://github.com/tronprotocol/tron-box).  

In addition, this contract should also run on the Ethereum virtual machine with few or no modifications.
#Usage

To install the dependencies, run

```npm install```

You can pick a password by swapping it out for the provided one in the contract.
You can deposit funds by sending to the generated contract address.

Then, configure the tronWeb object with a valid tron wallet.

If you redeployed the contract, you can swap out the provided contract address for the one generated by your contract migration. Put your password in the withdraw function, and specify how much you want to withdraw in units of Suns with 1,000,000 Suns being 1 tron.

You should then be good to go.  You should adjust the Fee Limit and Call Value if you get OUT OF ENERGY errors.  

Finally, the shouldPollResponse parameter of the function call will make the console wait for a response.  I prefer to have it set to true.
