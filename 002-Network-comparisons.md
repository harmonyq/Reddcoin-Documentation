# 2. Comparison with other blockchain networks
Historically, Reddcoin originated as a fork of Litecoin and Bitcoin, changed functionalities and protocol to migrate Proof-of-Stake. Reddcoin was invented as a response to increasing concerns about the efficiency of the Bitcoin PoW consensus model, as well as its increasing centralization and conflict of interests between miners. Reddcoin keeps much of the core code from Bitcoin, though it fundamentally changes the consensus model as well as introducing a number of new protocol paradigms and economics, including breaking the deflationary model of Bitcoin in favor of a sane and accountable level of inflation.

The fee market is also a subject where Reddcoin and Bitcoin differ. By moving to a fixed-fee model, the entire perspective of the blocksize limit and blockchain bandwidth is flipped upside down. While Bitcoin has a fee market by which miners (PoW block creators) are paid to process transactions so that the total supply can remain deflationary, in Reddcoin the minters (PoSV v2 block creators) are always rewarded for their participation with a proportional amount of inflation. As such, Reddcoin is free to burn the transaction fees such that the virtual-revenue of a transaction is shared by the entire network. By looking at the bandwidth problem as a community rather than individual nodes, we adopt a fixed fee level of 0.01 RDD/KB that allows for long-term prediction of transaction fee costs. The entirety of Reddcoin's blockchain is on the order of 6.5 GB, so blocksize limitations have never been tested. However, there is vast consensus in the community that if the blocksize approached the current limit, the limit would be lifted.
 
 
<table>
<thead>
<tr>
<th>Features</th>
<th>Bitcoin</th>
<th>Reddcoin</th>
<th>Ethereum</th>
</tr>
</thead>
<tbody>
<tr>
<td>Main use-case:</td>
<td>p2p financial transactions / store of value</td>
<td>p2p financial transactions / store of value</td>
<td>Turing complete smart contracts</td>
</tr>
<tr>
<td>Consensus algorithm:</td>
<td>PoW</td>
<td>PoSV v2</td>
<td>PoW</td>
</tr>
<tr>
<td>Active since:</td>
<td>2009</td>
<td>2014</td>
<td>2015</td>
</tr>
</tr>
<tr>
<td>Distribution method:</td>
<td>PoW block reward</td>
<td>(PoW block reward from Jan 2014 – Aug 2014: Terminated)</br>
PoSV v2 block reward
</td>
<td>Initial Coin Offering / PoW block reward</td>
</tr>
<tr>
<td>Distribution:</td>
<td>Limited, until 21M tokens exist in the system.</td>
<td>Unlimited.</td>
<td>Unlimited.</td>
</tr>
</tr>
<tr>
<td>Transaction fee:</td>
<td>Fee market (~100 satoshis/byte, ~$20/txn)</td>
<td>Fee market (~0.00028 RDD/byte, $0.000073)</td>
<td>Fee market (~100 Gwei/byte, ~$20/txn)</td>
</tr>
<tr>
<td>Estimated transaction bandwidth:</td>
<td>7 tx/sec</td>
<td>70 tx/sec</td>
<td>25 tx/sec</td>
</tr>
<tr>
<td>Block time:</td>
<td>10 minutes</td>
<td>1 minute</td>
<td>12 seconds</td>
</tr>
<tr>
<td>Block size:</td>
<td>1MB</td>
<td>1MB</td>
<td>Dynamic</td>
</tr>
<tr>
<td>Extra transaction data size limit:</td>
<td>80 Byte<br />(OP_RETURN)</td>
<td>80 Byte<br />(OP_RETURN)</td>
<td>Dynamic<br />(5 gas / byte)</td>
</tr>
<tr>
<td>Topology:</td>
<td>Public blockchain</td>
<td>Public blockchain</td>
<td>Public blockchain</td>
</tr>
</tbody>
</table>

Table 1. Comparison of Crypto currency attributes (prices of transactions at the time of writing)
