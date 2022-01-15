# Attak 1+2
* [Notebook](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%201%2B2/Attack_1_%2B_2.ipynb)

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
We can see after 10000 simulations, the number of created blocks for each probability. For Example: When the attacker has 20% of the network =>
- In 10000 time of attack, 12000 blocks are created.
- under 2000 blocks come from him
- In theory, he should create 2400 blocks

So if, the attaker don't have the minimum break-even point of the power, he should be an honnest miner.

![Adv_b](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%201%2B2/Adv_b.JPG)

After Having more than 41.4% (minimum break-even point) power of the Network, The attaker can mine more block than his mining power. Having 41.4% power of the network, at mean, 41.4% of blocks on the blockchain come from the attaker. 

![Adv_r](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%201%2B2/Adv_r.JPG)

And between 46% and 47% power of the Network, 50% of blocks on the blockchain come from him !

OverView on Reward per block
![Adv_w](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%201%2B2/Adv_w.JPG)

## Conclusion
You don't need 51% power of the Network tbe profitable, with the Attack 1+2, only 41.4% is sufficient
