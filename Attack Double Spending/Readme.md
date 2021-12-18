# Attak Double Spending

## Description
By Double Spending, a miner (or group of miners) increases their revenue by strategically withholding and releasing blocks to the network.
By not broadcasting their block right away, though, these miners effectively create their own private branch of the blockchain. The rest of the network continues to build on the previous block, while the selfish miner builds on top of this new chain. From that point, both chains will look completely different.
The goal of the Attaker is to always remain at least one block ahead of the rest of the network. Nodes accept the chain with the most accumulated proof of work as the valid blockchain. At any time, the Attaker can reveal their chain. If it is longer than the one followed by the rest of the network, the existing blocks will be discarded, and transactions reversed. The miner collects all of the rewards from these blocks and causes other parties to waste resources.

![intro](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/intro.JPG)

## Probability
### See the impact of the length of the network chain
#### a) minimum break-even point
We can see that the attacker should compete with the network without a long late. The attacker can reduce his need of power if he would compete against the network with small late.

![LenNet](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/LenNet.JPG)
```
Valeur min de Rdt Z=2 A=3 =>  0.44
Valeur min de Rdt Z=2 A=5 =>  0.46
Valeur min de Rdt Z=2 A=10 =>  0.47000000000000003
```

#### b) Advantages
<table>
  <tr>
    <td>Target(Z target attacker / A target Network)</td>
    <td>Z2_A3</td>
     <td>Z2_A5</td>
     <td>Z2_A10</td>
  </tr>
  <tr>
    <td>Blocks possession</td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_pZ2A3.JPG"></td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_pZ2A5.JPG"></td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_pZ2A10.JPG"></td>
  </tr>
  <tr>
    <td>Blocks ratio</td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_rZ2A3.JPG"></td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_rZ2A5.JPG"></td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_rZ2A10.JPG"></td>
  </tr>
  <tr>
    <td>Reward per simulation</td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_wZ2A3.JPG"></td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_wZ2A5.JPG"></td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_wZ2A10.JPG"></td>
  </tr>
 </table>
 
In Summary of this table, Attaker should not be very last if he want to be profitable with the smallest power of the network. But he will earn less. More the length of the network still increases more the number of mined blocks decreases, but the ratio of the network will increases.



### See the impact of the length of the attaker chain

#### a) minimum break-even point
We can see that the attacker should compete with the network without a big ambicious. The attacker can reduce his need of power if he would compete against the network with small lead.


![LenAtt](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/LenAtt.JPG)
```
Valeur min de Rdt Z=2 A=5 =>  0.46
Valeur min de Rdt Z=5 A=5 =>  0.49
with Z=10 and A=5 => +0.5
```


#### b) Advantages
<table>
  <tr>
    <td>Target(Z target attacker / A target Network)</td>
    <td>Z2_A5</td>
     <td>Z5_A5</td>
     <td>Z10_A5</td>
  </tr>
  <tr>
    <td>Blocks possession</td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_pZ2A5.JPG"></td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_pZ5A5.JPG"></td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_pZ10A5.JPG"></td>
  </tr>
  <tr>
    <td>Blocks ratio</td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_rZ2A5.JPG"></td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_rZ5A5.JPG"></td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_rZ10A5.JPG"></td>
  </tr>
  <tr>
    <td>Reward per simulation</td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_wZ2A5.JPG"></td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_wZ5A5.JPG"></td>
    <td valign="top"><img src="https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/AvantageImage/adv_wZ10A5.JPG"></td>
  </tr>
 </table>
 
 In Summary of this table, Attaker should not be arrogant (try to have lot of advance) if he want to be profitable with the smallest power of the network. But he will earn less. More the length of the attacker still increases more the number of mined blocks increases, but the ratio of the network will stay around 100% for long time.

### See the impact of the length

#### a) minimum break-even point
It's not very interresting for an attaker to compete the network with the same target. 
* More the target increase, more the attaker will be profitable very late. So, the idea to have a target more important than the network will be more profitable.
* More the target decrease, more the attaker will be profitable very soom. But, the profitabily is less interresting than the first idea (increase the target of the network).

![LenAtt](https://github.com/redek-zelton/Cryptofinance/blob/main/Attack%20Double%20Spending/Lensame.JPG)

## Conclusion
This attack is efficient because, you don't need 51% of the network. You need at least 44% of the power of the network to be profitable.
Howerver there is a gap of advantage between 44% and 48%.




