termine: TXID (IDENTIFICATORE DI TRANSAZIONE)

Un identificatore unico associato a ciascuna transazione Bitcoin. Viene generato calcolando l'hash `SHA256d` dei dati della transazione. Il TXID funge da riferimento per trovare una specifica transazione all'interno della blockchain. È utilizzato anche per fare riferimento a un UTXO, che è sostanzialmente la concatenazione del TXID di una transazione precedente e l'indice dell'output designato (chiamato anche "vout"). Per le transazioni post-SegWit, il TXID non prende più in considerazione la testimonianza della transazione, eliminando così la malleabilità.