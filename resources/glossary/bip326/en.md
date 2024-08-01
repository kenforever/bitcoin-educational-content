---
term: BIP326
---

A proposal for improvement aimed at developers of Bitcoin wallet software that supports Taproot transactions. Its main goal is to enhance the privacy of second-layer protocols that might use PTLCs (*Point Time Locked Contracts*), such as CoinSwap, the Lightning Network, or DLCs (*Discreet Log Contracts*). To achieve this, the proposal seeks to create plausible deniability by automatically configuring the `nSequence` field of Taproot transactions in the same manner as the `nLocktime` field was configured in other types of transactions to discourage fee sniping attacks. In other words, BIP326 asks wallet software to use the `nSequence` field instead of the `nLocktime` field to prevent fee sniping attacks, in order to provide increased privacy for all off-chain protocols using this field in a similar manner. Thus, a Taproot transaction with a specific value in the `nSequence` field could either be a standard wallet expenditure or a settlement transaction of a second-layer protocol with a time lock, making these two cases indistinguishable. If this improvement proposal is widely adopted by Bitcoin wallet software developers, it would greatly improve the privacy and fungibility of Bitcoin overall.
