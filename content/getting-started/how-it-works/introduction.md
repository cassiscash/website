+++
title = "Introduction"
draft = false
weight = 10
sort_by = "weight"
template = "page.html"

[extra]
toc = true
top = false
+++

# Introduction

Cassis relies on a central server, and yet it is **not custodial**. Or at least the server doesn't keep any custody of funds, but the entire thing works based on trust: not trust between users and the server, but between users and other users.

Let's take the example of **Alice** and **Bob**. They are friends and Bob is comfortable with Alice owing him **100,000**  satoshis. Each will generate a Schnorr keypair and share the public keys with each other, then Bob will reach out to the Cassis server and send a signed message that says, roughly:

```
<bob>: TRUST <alice> 100000
```

And with that a _trustline_ will be established between these two.

Now they can send transactions to each other using Cassis. First Alice can send transactions to Bob with

```
<alice>: TRANSFER <bob> 5000
```

and now Bob has up to **5,000** credit she can send back to Bob:

```
<bob>: TRANSFER <bob> 1337
```

And if you ask the Cassis server it will tell you right away that now **Alice owes Bob 93663** satoshis.

---

This is all very simple, but it's not adding much. How do we do actual payments, transfers that aren't between close friends?
