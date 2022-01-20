# Stratégie de block avec Optimisation
Deux versions:
* [Google Colab Redek Zelton](https://colab.research.google.com/drive/153FhEKBz2MZw9glTCGRPzJe7Hfoe-wFZ?usp=sharing)
* [Notebook](https://github.com/redek-zelton/Cryptofinance/blob/main/Strategie%20de%20block/Strat%C3%A9gie_de_block.ipynb)

## Description
Two teams of miner: Attaker and the Network.

They start with 0 block, and by a random process they can get blocks.

This strategy should optimise as max possible for the attaker, like a deep learning process.

![desc](https://github.com/redek-zelton/Cryptofinance/blob/main/Méthode%20de%20Minage%20Optimal/desc.JPG)

Rules:
* E(a,h,n,q,c): a(the number of blocks from Attaker), h(the number of blocks from Network), n(number of action to create a new block), q(power of the attacker), c(cost of mining)
* there are n possible blocks to create
* if the number of blocks from attacker is more or same than the Network => Publishes in the blockchain and erases all block mining during the attack from the network or Continue to mine.
* if the number of blocks from attacker is less than the Network => Abondones or Continue to mine.

* Abandon: (a,h) => (0,0) | reward = 0 and c = 0
* Publish: (a,h) => (a-h-1,0) | reward = h+1 and c = q
* Continue: (a,h) => (a+1,h) or (a,h+1) | reward = 0 and c = 0 or reward = 0 and c = q

## Formula
### Case when the simulation finishes with a=0 or abandon
* a > h+1
E(a,h,n,q,c) = Max( h+1-c+E(a-h-1,0,n,q,c) , qE(a+1,h,n-1,q,c)+(1-q)(E(a,h+1,n-1,q,c)-c )
* a = h+1
E(a,h,n,q,c) = Max( h+1-c , qE(a+1,h,n-1,q,c)+(1-q)(E(a,h+1,n-1,q,c)-c )
* a < h
E(a,h,n,q,c) = Max( 0 , qE(a+1,h,n-1,q,c)+(1-q)(E(a,h+1,n-1,q,c)-c )

### Case when the simulation finishes with n=0


### Case with attacker, who pays for orphan blocks
* a > h+1
E(a,h,n,q,c) = Max( h+1-c(h+1)+E(a-h-1,0,n,q,c) , qE(a+1,h,n-1,q,c)+(1-q)(E(a,h+1,n-1,q,c)-c )
* a = h+1
E(a,h,n,q,c) = Max( h+1-c(h+1) , qE(a+1,h,n-1,q,c)+(1-q)(E(a,h+1,n-1,q,c)-c )
* a < h
E(a,h,n,q,c) = Max( 0 , qE(a+1,h,n-1,q,c)+(1-q)(E(a,h+1,n-1,q,c)-c )

## Case when the simulation finishes with a=0 or abandon
![sim12](https://github.com/redek-zelton/Cryptofinance/blob/main/Méthode%20de%20Minage%20Optimal/sim_12.JPG)

The probability of this process with number = 3 is the same as the attack 1+2. Because 1+2 is a particular case of this strategy.

![sim](https://github.com/redek-zelton/Cryptofinance/blob/main/Méthode%20de%20Minage%20Optimal/sim.JPG)

We can see with number = 12 between 33% and 34% power of the network should be profitable! So only 12 actions, this method is more profitable than others except selfish mining

## Case with attacker, who pays for orphan blocks

![sima12](https://github.com/redek-zelton/Cryptofinance/blob/main/Méthode%20de%20Minage%20Optimal/sima_12.JPG)

With the number = 3, the attak cans not be profitable.

![sima](https://github.com/redek-zelton/Cryptofinance/blob/main/Méthode%20de%20Minage%20Optimal/sima.JPG)

With the number = 12, the attak cans not be profitable.

To Conclude, for all n, the value will stay at 0 !

## Conclusion
This Method shows the most optimised option for an Attaker. More the number of actions increases, more he need in power decreases! But this method is complexe, and shows all possibility in deep. 
there are 5^number_of_actions possible combinaisons !
