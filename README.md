# Cryptofinance
This reposite gives a quick view on Bitcoin Process.

## Bitcoin
### What is ?
The Whitepaper was created in 2008. Appeared in 2009, is based on 
a technical infrastructure supposed to propose “a new space of freedom” 
according to its creators.
- TotalSupply : 21M BTC
- Consensus : POW (SHA-256)
- Reward : at first 50 BTC and divided by 2 every 4years

### What is Difficulty?
Difficulty is a measure of how difficult it is to 
find a hash below a given target.
The Bitcoin network has a global block 
difficulty. Valid blocks must have a hash below 
this target. Mining pools also have a 
pool-specific share difficulty setting a lower 
limit for shares.
- Type Difficulty : random nonce
- Block Time Hash : 10 min
- Difficulty change: every 2016 Blocks

### TD
- [Proof of Work Mining](https://github.com/redek-zelton/Cryptofinance/tree/main/Proof%20of%20Work%20Mining) => Show how proof of work it works 

- [Attack 1+2 Simulation](https://github.com/redek-zelton/Cryptofinance/tree/main/Attack%201%2B2) => Efficient from : 0.4142

- [Attack Double Spending](https://github.com/redek-zelton/Cryptofinance/tree/main/Attack%20Double%20Spending) => Efficient from: 0.44 (Depend on the length of the Network and the Attaker (best is attaker=2 and network=3))

- [Attack Selfish Mining](https://github.com/redek-zelton/Cryptofinance/tree/main/Attack%20Selfish%20Mining) => Efficient from: 0.33

- [Optimal Mining Strategy](https://github.com/redek-zelton/Cryptofinance/tree/main/Méthode%20de%20Minage%20Optimal) => Efficient with 12 actions: between 0.33 and 0.34 or less with n > 12
