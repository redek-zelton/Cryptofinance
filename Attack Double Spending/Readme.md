# Attak Double Spending

## Description
By Double Spending, a miner (or group of miners) increases their revenue by strategically withholding and releasing blocks to the network.
By not broadcasting their block right away, though, these miners effectively create their own private branch of the blockchain. The rest of the network continues to build on the previous block, while the selfish miner builds on top of this new chain. From that point, both chains will look completely different.
The goal of the Attaker is to always remain at least one block ahead of the rest of the network. Nodes accept the chain with the most accumulated proof of work as the valid blockchain. At any time, the Attaker can reveal their chain. If it is longer than the one followed by the rest of the network, the existing blocks will be discarded, and transactions reversed. The miner collects all of the rewards from these blocks and causes other parties to waste resources.

![intro](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/intro.JPG)

## Probability
### See the impact of the length of the network chain
![LenNet](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/LenNet.JPG)



### See the impact of the length of the network attaker
![LenAtt](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Selfish%20Mining/LenAtt.JPG)







