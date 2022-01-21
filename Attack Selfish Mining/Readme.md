# Attack Selfish Mining
* [Notebook](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/Attack_Selfish_Mining.ipynb)

## Description
It's possible that more than 1 miner mine a new block at the same time, then the network will be fork. So then, each chain will challenge each other. The longest chain will survive, and others will be destroyed.

The attaker should have an advance against honest miners. Regardless his advance, he mines secretly on his side. But when the advance is 1, he broadcasts immediately his blocks on the blockchain. Then it's erased all endevors from honnest miners during the attack.

But at first of his attack, if the network finds. then his advance is 0. the attacker abandons.

![intro](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/Intro.JPG)

## Minimum break-even point of power of mining
We give the probability table:

![Intro2](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/Intro2.JPG)

* The mean of the reward is ER
* The mean of the number of block is EH
* Rdt = ER/EH Then

![Sim](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/Sim.JPG)

The miner should only need 33% power of the network to be profitable.


## Advantage
During the simulation, we can see a strong exponential increase of blocks in the blockchain! This strong increase comes from the power of the attacker, because only he cans publish blocks. if no, the height still increases by 1.

![adv_b](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/adv_b.JPG)

After Having more than 33% power of the Network, The attaker can mine more block than his mining power. Having around 33% power of the network, at mean, 33% of blocks on the blockchain come from the attaker.

Around 40% power of the Network, 50% of blocks on the blockchain come from him.

![adv_r](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/adv_r.JPG)

And Near to 50% power of the Network, All blocks come from Attaker !!!

The reward can show use that the number of blocks can create an attaker when he tries selfish mining. For example: An attacker having 48% power of the network, at mean, he cans create 6 blocks! it's huge.

![adv_w](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/adv_w.JPG)


## Conclusion
This attack is efficient because, you don't need 51% of the network. Only 33% is sufficient to be profitable







* [Référence 1](https://hal.archives-ouvertes.fr/hal-01794067/document)
* [Référence 2](https://arxiv.org/pdf/1311.0243.pdf%7C)

