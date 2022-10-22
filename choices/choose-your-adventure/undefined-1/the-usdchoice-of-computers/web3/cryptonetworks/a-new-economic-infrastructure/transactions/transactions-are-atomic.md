---
layout: editorial
---

# Transactions are ⚛️-ic

### <mark style="color:purple;">Transactions are either successfully terminated or reverted:</mark>

### <mark style="color:orange;">1) From EOA to EOA: any changes to the global state are recorded (</mark>_<mark style="color:orange;">e.g.,</mark>_ <mark style="color:orange;"></mark><mark style="color:orange;">account balances).</mark>&#x20;

### <mark style="color:green;">2) From EOA to a contract that does not invoke other contracts: any changes to the global state are recorded (</mark>_<mark style="color:green;">e.g.</mark>_<mark style="color:green;">, account balances, state variables of the contracts).</mark>

### <mark style="color:red;">3) From EOA to a contract that invokes other contracts in a manner that propagates errors: any changes to the global state are recorded (</mark>_<mark style="color:red;">e.g.</mark>_ <mark style="color:red;"></mark><mark style="color:red;">account balances, state variables of the contracts).</mark>&#x20;

### <mark style="color:blue;">4) From EOA to a contract that invokes other contracts in a manner that does NOT propagates errors: there may be changes to the global state recorded (</mark>_<mark style="color:blue;">e.g.,</mark>_ <mark style="color:blue;"></mark><mark style="color:blue;">account balances, state variables of the non erroring contracts), whereas other changes are not recorded (</mark>_<mark style="color:blue;">e.g.</mark>_ <mark style="color:blue;"></mark><mark style="color:blue;">state variables of the erroring contracts).</mark>&#x20;

### <mark style="color:purple;">If a tx is reverted, all of its effects (changes in state) are "rolled back". A failed transaction is still recorded and the ether spent on gas for the execution is deducted from the originating account.</mark>
