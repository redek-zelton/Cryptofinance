# Attak Double Spending

## Description
By Double Spending, a miner (or group of miners) increases their revenue by strategically withholding and releasing blocks to the network.
By not broadcasting their block right away, though, these miners effectively create their own private branch of the blockchain. The rest of the network continues to build on the previous block, while the selfish miner builds on top of this new chain. From that point, both chains will look completely different.
The goal of the Attaker is to always remain at least one block ahead of the rest of the network. Nodes accept the chain with the most accumulated proof of work as the valid blockchain. At any time, the Attaker can reveal their chain. If it is longer than the one followed by the rest of the network, the existing blocks will be discarded, and transactions reversed. The miner collects all of the rewards from these blocks and causes other parties to waste resources.

![intro](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/intro.JPG)

## Probability
### See the impact of the length of the network chain
We can see that the attacker should compete with the network without a long late. The attacker can reduce his need of power if he would compete against the network with small late.

![LenNet](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/LenNet.JPG)
```
Valeur min de Rdt Z=2 A=3 =>  0.44
Valeur min de Rdt Z=2 A=5 =>  0.46
Valeur min de Rdt Z=2 A=10 =>  0.47000000000000003
```



### See the impact of the length of the attaker chain
We can see that the attacker should compete with the network without a big ambicious. The attacker can reduce his need of power if he would compete against the network with small lead.


![LenAtt](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/LenAtt.JPG)
```
Valeur min de Rdt Z=2 A=5 =>  0.46
Valeur min de Rdt Z=5 A=5 =>  0.49
with Z=10 and A=5 => +0.5
```







