# Attack Selfish Mining

## Description
It's possible that more than 1 miner mine a new block at the same time, then the network will be fork. So then, each chain will challenge each other. The longest chain will survive, and others will be destroyed.
The idea of this attak is to hide our chain, when the network is 1 block behind us, so we broadcast our chain. Then our chain will be valid, but not the network.

![intro](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/Intro.JPG)

## Minimum break-even point of power of mining
We give the probability table:

![Intro2](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/Intro2.JPG)

* The mean of the reward is ER => SUM(n*(p*q)^n) with n to +inf      =>      p*q / (1 - p*q)^2
* The mean of the number of block is EH => 1*p+SUM(n*(p*q)^n) with n to +inf    => p + p*q /(1- p*q)^2
* Rdt = ER/EH Then

![Sim](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/Sim.JPG)

The miner should only need 33% power of the network to be profitable.

## Minimum break-even point of power of mining after paying charges
After Paying charges, with 33% power of Network, the Attaker can generate profits. In Theory, it is a bit less than 33%.

![Rwd](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/Rwd.JPG)

## Advantage
After Having more than 33% power of the Network, The attaker can mine more block than his mining power. Having around 33% power of the network, at mean, 33% of blocks on the blockchain come from the attaker.

Around 38% power of the Network, 50% of blocks on the blockchain come from him.

![adv](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/adv.JPG)

And Near to 50% power of the Network, All blocks come from Attaker !!!
