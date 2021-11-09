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

The miner should only need 41.4% power of the network to be profitable. 

## Advantage
After Having more than 41.4% power of the Network, The attaker can mine more block than his mining power. Having 41.4% power of the network, at mean, 41.4% of blocks on the blockchain come from the attaker. 

![Adv](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%201%2B2/Adv.JPG)

And between 46% and 47% power of the Network, 50% of blocks on the blockchain come from him !

## Conclusion
You don't need 51% power of the Network tbe profitable, with the Attack 1+2, only 41.4% is sufficient
