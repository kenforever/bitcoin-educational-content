---
term: DOUBLE SPENDING (ATTACK)
---

An attack where a malicious user attempts to use the same UTXO (*Unspent Transaction Output*) more than once to enrich themselves at the expense of the parties involved in the transactions. In principle, once a transaction is confirmed in a block and added to the blockchain, the use of those bitcoins is permanently recorded, preventing any further spending of the same bitcoins. Preventing double spending is even the primary utility of the blockchain.

In the context of a double spending attack, the attacker first makes a legitimate transaction with a merchant, then creates a second competing transaction spending the same coins, either by sending them back to themselves to recover the amount or by using them to purchase another good or service from a different merchant.

There are two main scenarios that can enable this attack. The first, and simplest for the attacker, involves executing the fraudulent transaction before the legitimate transaction is included in a block. To ensure their fraudulent transaction is confirmed first, the attacker associates significantly higher transaction fees with it than with the legitimate transaction. This is a kind of fraudulent RBF. This scenario is only possible if the merchant agrees to finalize the sale in "zeroconf," meaning without any confirmations for the payment transaction. This is why it is strongly recommended to wait for several confirmations before considering a transaction as immutable. The second scenario, much more complex, is that of a 51% attack. If the attacker controls a significant portion of the network's computing power, they can mine a competing chain to the one containing the legitimate transaction, but including their fraudulent transaction. When the merchant has accepted the sale and the attacker has succeeded in creating a longer chain (with more accumulated work) than the legitimate chain, they can then broadcast their fraudulent chain, which will be recognized by the network nodes as the valid one.