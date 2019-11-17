# TON Blockchain Tolerant Personal Multisig

High performance multi-signature wallet intended to be used by a single user or
company. Executes messages in-order and mitigates attack when attacker
controls minority of keys, while owner controls all of them.

### Accepting out-of-order messages

Contract accepts messages out-of-order, but executes them in-order. It's in a
way similar to other blockchains. Owner may send many messages at once and they
will be buffered and re-ordered by contract.

### Containing attack

Contract is paying message processing fees and enforces limits on how many
resources can be consumed by an individual key.
