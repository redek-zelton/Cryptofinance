# Stratégie de block avec Optimisation
Deux versions:
* [Google Colab Redek Zelton](https://colab.research.google.com/drive/153FhEKBz2MZw9glTCGRPzJe7Hfoe-wFZ?usp=sharing)
* [Notebook](https://github.com/redek-zelton/Cryptofinance/blob/main/Strategie%20de%20block/Strat%C3%A9gie_de_block.ipynb)

## Description
Two teams of miner: Attaker and the Network.

They start with 0 blocks, and by a random process they can get blocks.

This strategy should optimise as max possible for the attaker, like a deep learning process.

Rules:
* E(a,h,n,q,c): a(the number of blocks from Attaker), h(the number of blocks from Network), n(number of action), q(power of the attacker), c(cost of mining)
* the number of action depend on n
* if the number of blocks from attacker is more or same than the Network => Publishes in the blockchain and erases all block mining during the attack from the network or Continue to mine.
* if the number of blocks from attacker is less than the Network => Abondones or Continue to mine.


## Méthode d'Optimisation Sans Ajustement des blocks
![sim12](https://github.com/redek-zelton/Cryptofinance/blob/main/Strategie%20de%20block/sim_12.JPG)

The probability of this process with number = 3 is the same as the attack 1+2. Because 1+2 is a particular case of this strategy.

![sim](https://github.com/redek-zelton/Cryptofinance/blob/main/Strategie%20de%20block/sim.JPG)

We can see with number = 12 only 33% power of the network should be profitable! So only 12 actions, this method is more profitable than selfish 

## Méthode d'Optimisation Avec Ajustement des blocks

![sima12](https://github.com/redek-zelton/Cryptofinance/blob/main/Strategie%20de%20block/sima_12.JPG)

The probability of this process with number = 3 is over 51%, because now the Attaker should pay all bills.

![sima](https://github.com/redek-zelton/Cryptofinance/blob/main/Strategie%20de%20block/sima.JPG)

The probability of this process with number = 12 is 51%. So when the number of actions increases, the attacker should decreases he needs in power. 

## Conclusion
This Method shows the most optimised option for an Attaker. More the number of actions increases, more he need in power decreases! But this method is complexe, and shows all possibility in deep.
there are 5^number_of_actions possible combinaisons !


