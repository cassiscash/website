+++
title = "Routed Payments"
draft = false
weight = 11
sort_by = "weight"
template = "page.html"

[extra]
toc = true
top = false
+++

# Routed Payments

Let's introduce **Charlie**, who trusts **Bob** up to **50,000**:

```
<charlie>: TRUST <bob> 50000
```

and **Derek**, who trusts **Charlie** up to **70,000** satoshis:

```
<derek>: TRUST <charlie> 70000
```

Now the Cassis server is aware of all these trust relationships, making it possible for it to compute a route between **Alice** and **Derek**, through which a payment of up to **50,000 satoshis** can be routed.

Suppose Derek has an online store that sells hats and he wants to accept payments using Cassis, so Derek can either create a new keypair for his store and trust his own personal key with it -- or, for simplicity, he can just use his personal keypair for the store.

Now when Alice visits _Derek's Hat Shop_ webpage and clicks to buy a hat she will be presented with an invoice for **24,277 satoshis**, which she fulfills:

```
<alice>: TRANSFER <derek> 24277
```

Since there is a route available the payment gets computed instantly and now the balances read like

```
<alice> owes <bob>: 27940
<bob> owes <charlie>: 24277
<charlie> owes <derek>: 24277
```

What do we do with all these debts now?
