term: BITVM

Protocollo introdotto da Robin Linus nel 2023, volto ad estendere le capacità di sviluppo applicativo di Bitcoin. BitVM consente l'esecuzione arbitraria di qualsiasi operazione computazionale e utilizza questa computazione per dirigere i bitcoin coinvolti. Il protocollo prevede lo spostamento di tutte le computazioni off-chain, consentendo al contempo che la computazione possa essere contestata on-chain se l'altra parte sostiene un risultato fraudolento. In questo modo, BitVM fornisce a Bitcoin una capacità computazionale quasi Turing-completa, senza richiedere modifiche a livello di consenso. BitVM replica il comportamento di un gate logico `NAND` attraverso l'uso combinato degli opcode `OP_BOOLAND` (che a sua volta replica il comportamento di un gate logico `AND`) e `OP_NOT` (che replica il comportamento di un gate logico `NOT`). Infatti, questo gate logico `NAND` può essere utilizzato nella catena per replicare il comportamento di tutti gli altri gate logici esistenti. Questo è ciò che viene chiamato un "gate universale". Per estensione, una serie di gate logici `NAND` può quindi replicare qualsiasi circuito computazionale. L'idea con BitVM è di memorizzare queste sequenze di computazione `NAND` come foglie nel MAST di una transazione Taproot.