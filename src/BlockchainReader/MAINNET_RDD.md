## Reading from the Bitcoin Blockchain

Po.et uses the `OP_RETURN` opcode to store a reference to batched claims. Any `OP_RETURN` data that begins with `POET` is assumed to be a `POET` message.

Following the `POET` protocol header, we specify a version using the next 2 bytes. The next byte is a protocol enum, followed by the data hash:

`POETVR0HASHGOESHERE`

```
Poet protocol  version  prototol  data hash
POET           VR       0         HASHGOESHERE
```
