# GateKeeperTwo
Here's how I passed each modifier
## gateOne
I used a contract to call the Gatekeeper Contract making my address the `tx.origin` and my contracts address the `msg.sender`

## gateTwo 
During a contracts creation it doesn't have any code associated with its calculated address until after the execution of its constructor function. So I made the call inside the constructor function when it had no code associated with its address.

## gateThree
Reversed the exclusive-Or(^) operation to get the `_gateKey` and sent it as an argument to the call.

You can check [here](https://medium.com/coinmonks/ethernaut-lvl-14-gatekeeper-2-walkthrough-how-contracts-initialize-and-how-to-do-bitwise-ddac8ad4f0fd) for an indepth analysis of the challenge.
