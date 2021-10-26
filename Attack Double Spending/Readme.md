# Attak Double Spending

## Description
It's possible that more than 1 miner mine a new block at the same time, then the network will be fork. So then, each chain will challenge each other. The longest chain will survive, and others will be destroyed.
The idea of this attak is to hide our chain, when the network is 1 block behind us, so we broadcast our chain. Then our chain will be valid, but not the network.


## Probability
We give the probability table:


* The mean of the reward is ER => SUM(n*(p*q)^n) with n to +inf      =>      p*q / (1 - p*q)^2
* The mean of the number of block is EH => 1*p+SUM(n*(p*q)^n) with n to +inf    => p + p*q /(1- p*q)^2
* Rdt = ER/EH Then



The miner should only need 33% power of the network to be profitable.
