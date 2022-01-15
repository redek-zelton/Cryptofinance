# Proof of Work
* [Notebook](https://github.com/redek-zelton/Cryptofinance/blob/main/Proof%20of%20Work%20Mining/Proof_of_Work_Mining.ipynb)

## Concept
Bitcoin as a permission-less blockchain uses
proof-of-work. 
PoW is a cryptographic puzzle that is difficult to solve but easy to verify. More you have computing power, more your reward is high.
However, significant latency of proof-of-work for transactions confirmation has negative effects on blockchain security such that longer delays may increase the number of forks and the possibilities for mounting double-spending attacks.


## block
 Bitcoin difficulty changes every 2016 blocks.
 New_d = Old_d x (time last 2016 / (2016 x mean_time_for_1_block))


## block mining follow an exponential function
 Each hash is 256 bits => 32 Bytes in Hex (0 => F)
 So to have an Hash with 0.............., we need to hash 16 times in mean.
 then the nonce follow this :
- Difficulty 0 => 16^0 => 1
- Difficulty 1 => 16^1 => 16
- Difficulty 2 => 16^2 => 256
- Difficulty 3 => 16^3 => 4096 ...
- Difficulty 16 => 16^16 => 18 446 744 073 709 551 616
- Difficulty 32 => 32^16 => 3,403e+38 (get collision)

![f_expo](https://github.com/redek-zelton/Cryptofinance/blob/main/Proof%20of%20Work%20Mining/f_expo.JPG)
* In Theory => So we can conclude the block mining for this function f(d) = 16^d, where d is the difficulty (number of zeros)
* In Reality => it is f(d) = 16^(d-1)*(16/2) because in the last case, we have 50% chance


## Time of found a specific block follow an exponential law
 Hash many time for a specific difficulty didn't give the same nonce or the same time of hash.
 It follows a continuous variable probability => P(T>t) with T is the time of hash, and t the target.
 
 ![l_expo](https://github.com/redek-zelton/Cryptofinance/blob/main/Proof%20of%20Work%20Mining/l_expo.JPG)
 We can see : 
 - P(T>0) ==> 1
 - P(T> +inf) ==> 0
 
 ![lien](https://github.com/redek-zelton/Cryptofinance/blob/main/Proof%20of%20Work%20Mining/lien.JPG)
 
 By using Kolmogorov-Smirnov(K-S) test, we can see the link between hash and exponential law.
 
## Applications
In the part 3 (Applications), we can make some test, and try to find a time for a probability or vise-versa.
 




