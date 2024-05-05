+++
title = "What if bad things happen?"
draft = false
weight = 50
sort_by = "weight"
template = "page.html"

[extra]
toc = true
top = false
+++

# What if bad things happen?

There are two bad things that can happen with Cassis users: (1) a debtor might default on their debt; or (2) the Cassis server may go rogue.

## A debtor defaults on their debt

If this happens to you there is nothing that can be done. The good thing is that you shouldn't have trusted them with too much money and hopefully you lost only a little bit. Perhaps the amount you lost is still smaller than the price of a Lightning Channel unilateral close in a high-fee environment.

## The Cassis server goes rogue

If the Cassis server goes rogue, goes offline, or starts publishing a completely invalid and different state from what it had previously published, you -- or another server or service you instructed to keep track of these things on your behalf and didn't go rogue -- still have the latest valid state between you and your peers, and that debt is still valid. You can just agree with your peers to migrate these states to a different Cassis server, or settle them manually and move on with your lives.
