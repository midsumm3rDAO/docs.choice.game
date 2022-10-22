---
layout: editorial
---

# The structure of a tx

### <mark style="color:purple;">A transaction is a</mark> <mark style="color:orange;">serialized</mark> <mark style="color:purple;"></mark> <mark style="color:orange;">binary</mark> <mark style="color:purple;"></mark> <mark style="color:orange;">message</mark> <mark style="color:purple;">that contains:</mark>

### <mark style="color:green;">1. nonce (prevent message replay)</mark>

### <mark style="color:green;">2. gas price (amount of ether the originator is willing to pay)</mark>

### <mark style="color:green;">3. gas limit (maximum gas the originator is willing to buy)</mark>

### <mark style="color:green;">4. recipient (destination Ethereum address)</mark>

### <mark style="color:green;">5. value (amount of ether to send to the destination)</mark>

### <mark style="color:green;">6. data (variable-length binary data payload)</mark>

### <mark style="color:green;">7. v, r, s (components of an ECDSA digital signature of the originating EOA)</mark>
