+++
title = "Settlement"
draft = false
weight = 11
sort_by = "weight"
template = "page.html"

[extra]
toc = true
top = false
+++

# Internal Settlement

Whenever someone owes someone else money on Cassis, it doesn't follow that they have to make some kind of external settlement. The person who has the credit can always automatically use it inside the network by sending transfers through existing _trustlines_ that go through the debtor, either to buy other things or to perform a circular rebalance and settle their own debts on _trustlines_ on the other side.

# Dynamic Settlement

Debts might also be settled dynamically, by the natural shift of transfers from third-parties.

In the previous page we saw that a payment from Alice to Derek caused balances to shift all over the network, affecting Bob and Charlie too. In a bigger Cassis network, these events would be very common and payments would flow through existing _trustlines_ in both directions, so it is entirely plausible that Alice will go to sleep owing **27,940** to Bob, but when she wakes up she owes nothing to Bob anymore but instead owes 20,000 to Zooey and 7,940 to Yuri.

# External Settlement

However it may also be that Alice has received a _trustline_ of 500,000 satoshis from Erin and after some days or weeks and many transactions that gets filled up such that now **Alice owes 477,183 satoshis to Erin**. Now it might make sense for Alice to pay that debt so her trustline gets cleaned up. She can do using a normal Bitcoin transaction, a Lightning Network transaction, direct fiat cash or any other means. She can pay it in full, partially, or even overpay. And these actions should be reflected in the trustline state and balances.

Suppose Alice has talked to Erin and then paid her **500,000 satoshis** in a Bitcoin transaction, which Erin then reports as a normal transfer:

```
<erin>: TRANSFER <alice> 500000
```

After that the state will be that **Erin now owes Alice 22,817 satoshis**.
