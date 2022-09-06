# Proof-of-Stake

>Reddcoin uses Proof-of-Stake algorithms. ………..The PoW algorithm is used to spread the distribution of new coins. Up to 99% of all Reddcoins is created with PoW. Proof-of-Stake is used to secure the network: The chain with longest PoS coin age wins in case of a blockchain split-up.

Staking, as it is called in Reddcoin to make a proof-of-stake block, is based on metrics of an unspent transaction. If we take a look at the number one spot of the rich list, transaction c7293fc60c80bdcc374775d1f0734e0766465b905bae1a312fe487793be3b8f7 has among others the following characteristics:
*	The transaction appeared in block 376161 at timestamp 1531750952 (Unix time).
*	The transaction in the block has an offset of 383 bytes. It is the third transaction in the block. The size of the first two transactions in the block are respectively 78 and 224 bytes.
*	The transaction timestamp is 1531750624. (As of Reddcoin 0.11, the block timestamp is to be used instead of the transaction timestamp)
*	The second recipient (index 1) received 1786301.06651300 Reddcoins which, at the moment, is still unspent.
These metrics, along with two more data points serves as a basis to calculate a hash for POS minting:
*	a future timestamp X (in Unix time notation) in which the stake could win;
*	a block modifier that was set by the network 1830080 seconds (~21 days) earlier than X.
Every 6 hours the network calculates a new block modifier to be used for POS minting.
The win in proof-of-stake minting, the calculated hash is compared to the current difficulty minus the coinage. The chances of finding a stake therefor improves when either the coin age increases or when the difficulty of the network decreases.

## Reddcoin staking behaviour
*	The Staking process can only start after 8 hours of coinage.
*	Staking coin age is maxed out after 90 days. Which means that after 90 days the only variable left in PoS is the current difficulty.
*	Staking is predictable and not random. For a given transaction, you can calculate the maximum network PoS difficulty over time for your transaction to be able to mint a PoS block.
*	Whenever this PoS difficulty is higher than the current network PoS difficulty your Reddcoin client can mint a PoS block.
*	PoS blocks can be rejected (orphans) if several people mint a PoS block within a given window (2 hours also called timedrift). Only one (the chain with longest coin age) will be accepted.
*	Minting splits the transaction in two if coin age < 90 days.
*	PoS block reward is 3% + 0.25 RDD per solved block. See RFC0018 for more details RFC0018
*	A transaction that just staked has its coins locked for 520 confirmations (3-4 days).
*	Merging transactions, spending coins, etc. burns coinage (resets it to 0).
*	The PoS reward is directly added to your transaction which staked (if this transaction is split in two because coinage < 90 days, the reward is equally distributed to both resulting transactions).
 
Qualities of Proof-of-Stake Consensus
Efficient
Proof-of-Stake (PoS) is an alternative to PoW first introduced in Peercoin . The resource used by PoS is “coin age": currency amount times holding period. Similar to energy, coin age as a resource is expensive to amass in huge quantity. For an attacker to accumulate enough coin age to attack the distributed network, he either has to buy on open market a large amount of the very currency he's trying to attack, driving up its price during the process and diminishing his economic incentive, or hold coins for a very long time, reducing the frequency of his own attacks.
One useful feature of PoS is the significant savings in energy consumption. Another main feature is the better alignment of incentives between miners and stakeholders because miners are now the stakeholders.

## Qualities of Proof-of-Stake Consensus

### Efficient

Proof-of-Stake (PoS) is an alternative to PoW first introduced in Peercoin . The resource used by PoS is “coin age": currency amount times holding period. Similar to energy, coin age as a resource is expensive to amass in huge quantity. For an attacker to accumulate enough coin age to attack the distributed network, he either has to buy on open market a large amount of the very currency he's trying to attack, driving up its price during the process and diminishing his economic incentive, or hold coins for a very long time, reducing the frequency of his own attacks.

One useful feature of PoS is the significant savings in energy consumption. Another main feature is the better alignment of incentives between miners and stakeholders because miners are now the stakeholders.

### Aligning interests
Because coin owners also produce new blocks in our Proof-of-Stake protocol consensus algorithm, this means security providers and users of the network are ultimately the same group of people. No longer is there a separate group of security providers who only care about making profit and are not financially tied to the network itself. All security providers must own a stake in the network through ownership of Reddcoin. As everyone has similar financial interests in the long-term future of the network this leads to much less conflict between factions with different ideas about how the blockchain should develop and evolve.

### User governance
Because users in Reddcoin have the ability to produce blocks they also have the power to influence and determine the future direction of the network. User governance goes hand in hand with the PoS consensus mechanism. Reddcoin is a blockchain capable of allowing its protocol rules to be governed directly by its users.

### Global network
As a direct consequence of the resource efficient consensus mechanism the number of people capable of participating in the race to create new blocks is the same users having their stake. In addition to this security providers are also no longer drawn to geographical locations with cheap electricity. Due to the cost efficiency of operating a proof-of-stake node minting nodes can be set up anywhere in the world. This allows Reddcoin to maximize its level of decentralization and achieve global security from staking users all around the world.

### Network security is price independent
Unlike proof-of-work where miners are completely dependent on the market price of a blockchain's native token to ensure profitability, Reddcoin contains no such price dependency. Stake owners are compensated as motivation to provide consistent security, however since this process is so inexpensive to perform staking actually have the ability to voluntarily operate a minting node without compensation if they want. Even without compensation from the network, the process of staking helps to secure the blockchain and along with it a stakeholder's overall investment. The ability to decide which version of the protocol to run also gives a stakeholders the opportunity to make their voice heard concerning future upgrades to the network. These are two important reasons a stakeholder may have to want to secure the network, however, compensation is automatically provided which makes it even better to participate. Running a proof-of-work mining node without compensation is just not possible due to the requirement of being profitable enough in order to afford the associated costs of participating. However, since 2014 it has been proven that Reddcoin is capable of sustaining its network security even during the lowest periods of demand where market price was close to zero. If the network is capable of surviving extremely stressful conditions like these then it is likely to survive any challenges the market may present it with in the future.

### Higher Resistance to Censorship

As explained above, the efficiency of proof-of-stake results in a blockchain network that can easily be secured by people all over the world who hold some amount of Reddcoin. This globally decentralized security makes the Reddcoin network incredibly difficult to censor and shut down. This is similar to downloading files through a bittorrent network. In bittorrent network, many people around the world operate nodes where they hold a full copy of the file that others are trying to download. Pieces of the file are downloaded from different nodes until the full file has finished downloading. If a government were to deem this file sharing illegal and attempt to shut down the torrent network, they would be forced to target every single node on the network no matter where they happen to exist in the world. Even then, there is nothing stopping more torrent nodes from being created that share the same file. As long as one node exists that shares the file, it can be downloaded and spread to others.
Reddcoin works in a similar way where stakers that process transactions can be operated from anywhere in the world as long as the stake owners has access to a computer, minimal electricity, some amount of Reddcoin and an internet connection. Geographical decentralization of staking makes it incredibly difficult to shut down the Reddcoin network, but when the number of nodes around the world expands to thousands or even tens of thousands then it essentially becomes impossible to censor. In systems like these, individual nodes are usually called peers. Together they act as a peer-to-peer network. This is where Reddcoin obtained its name. It was originally introduced by Sunny King as ppcoin, which stood for peer-to-peer coin. Shortly after it was renamed to Reddcoin.
