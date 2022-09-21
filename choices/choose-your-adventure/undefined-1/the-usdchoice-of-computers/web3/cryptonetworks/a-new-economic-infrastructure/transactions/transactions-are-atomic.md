---
layout: editorial
---

# Transactions are atomic

### <mark style="color:purple;">Transactions are either successfully terminated or reverted:</mark>

### <mark style="color:orange;">1) From EOA to EOA: any changes to the global state are recorded (e.g., account balances).</mark>&#x20;

### <mark style="color:green;">2) From EOA to a contract that does not invoke other contracts: any changes to the global state are recorded (e.g., account balances, state variables of the contracts).</mark>

### <mark style="color:red;">3) From EOA to a contract that invokes other contracts in a manner that propagates errors: any changes to the global state are recorded (e.g. account balances, state variables of the contracts).</mark>&#x20;

### <mark style="color:blue;">4) From EOA to a contract that invokes other contracts in a manner that does NOT propagates errors: there may be changes to the global state recorded (e.g., account balances, state variables of the non erroring contracts), whereas other changes are not recorded (e.g. state variables of the erroring contracts).</mark>&#x20;

### <mark style="color:blue;">I</mark><mark style="color:purple;">f a tx is reverted, all of its effects (changes in state) are "rolled back".</mark>&#x20;

### <mark style="color:purple;">A failed transaction is still recorded and the ether spent on gas for the execution is deducted from the originating account.</mark>
