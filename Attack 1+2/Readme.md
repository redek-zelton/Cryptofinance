# Attak 1+2

## Description
The Attaker chooses to attack during 3 blocks. If the first block is mined by the network, the attaker would stop immediatly. But if the first block is mined by him, he would challenge the network for 2 blocks.

![intro](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%201%2B2/Intro.JPG)


## Probability
We give the probability table

![intro2](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%201%2B2/intro2.JPG)
* The mean of the reward is ER => 3*q^3 + 4*p*q^2
* The mean of the number of block mined is EH => 1*p + 3*q^3 + 4*p*q^2 + 2*p^2*q
* Rdt = ER/EH
Then

![proba](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%201%2B2/proba.JPG)

The miner should only need 41,4% power of the network to be profitable. 
