# 2. Comparison with other blockchain networks
Historically, Reddcoin originated as a fork of Litecoin and Bitcoin, changed functionalities and protocol to migrate Proof-of-Stake. Reddcoin was invented as a response to increasing concerns about the efficiency of the Bitcoin PoW consensus model, as well as its increasing centralization and conflict of interests between miners. Reddcoin keeps much of the core code from Bitcoin, though it fundamentally changes the consensus model as well as introducing a number of new protocol paradigms and economics, including breaking the deflationary model of Bitcoin in favor of a sane and accountable level of inflation.

The fee market is also a subject where Reddcoin and Bitcoin differ. By moving to a fixed-fee model, the entire perspective of the blocksize limit and blockchain bandwidth is flipped upside down. While Bitcoin has a fee market by which miners (PoW block creators) are paid to process transactions so that the total supply can remain deflationary, in Reddcoin the minters (PoSV v2 block creators) are always rewarded for their participation with a proportional amount of inflation. As such, Reddcoin is free to burn the transaction fees such that the virtual-revenue of a transaction is shared by the entire network. By looking at the bandwidth problem as a community rather than individual nodes, we adopt a fixed fee level of 0.01 RDD/KB that allows for long-term prediction of transaction fee costs. The entirety of Reddcoin's blockchain is on the order of 6.5 GB, so blocksize limitations have never been tested. However, there is vast consensus in the community that if the blocksize approached the current limit, the limit would be lifted.
 
 
Features	Bitcoin	Reddcoin	Ethereum
Main use-case:	p2p financial transactions / store of value	p2p financial transactions / store of value	Turing complete smart contracts
Consensus algorithm:	PoW	PoSV v2	PoW
Active since:	2009	2014	2015
Distribution method:	PoW block reward	(PoW block reward from Jan 2014 – Aug 2014: Terminated.)
PoSV v2 block reward	Initial Coin Offering / PoW block reward
Distribution:	Limited, until 21M tokens exist in the system.	Unlimited.	Unlimited.
Transaction fee:	Fee market (~100 satoshis/byte, ~$20/txn)	Fee market (~0.00028 RDD/byte, $0.000073)	Fee market (~100 Gwei/byte, ~$20/txn)
Estimated transaction bandwidth:	7 tx/sec	70 tx/sec	25 tx/sec
Block time:	10 minutes	1 minute	12 seconds
Block size:	1MB	1MB	Dynamic
Extra transaction data size limit:	80 Byte
(OP_RETURN)	80 Byte
(OP_RETURN)	Dynamic
(5 gas / byte)
Topology:	Public blockchain	Public blockchain	Public blockchain
Table 1. Comparison of Crypto currency attributes (prices of transactions at the time of writing)
