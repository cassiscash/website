+++
title = "Other Remarks"
draft = false
weight = 100
sort_by = "weight"
template = "page.html"

[extra]
toc = true
top = false
+++

# On the enforceability or social validity of the debts

Keep in mind that these debts are not enforceable by any means, and they do not even imply that Alice has agreed to pay Bob. Bob is the one who initiated the trust relationship, and he should only have done that if he is comfortable and in agreement with Alice about their obligations.

A system of contracts and reputation for users of Cassis is outside the scope of the protocol.

# On the privacy of the system

Cassis is remarkably bad for privacy. It's at the level of having an Ethereum address that can be publicly related to a person, infinitely reused.

One argument that ameliorates the situation is that Cassis is only intended to be used by normal people for small amounts, day-to-day payments, buying coffee and so on, so an attacker should not be able to learn much about the actual wealth of a user or of their bigger transfers that will use normal Bitcoin transactions or other means.

Data about individual payments can also theoretically be obfuscated by using a kind of "coinjoin" that lumps together multiple transfers from multiple people, such that it's not clear who is paying whom. This can be automated by some third party and made easy to use.

Fully closed Cassis registries would solve these issues, but by not publishing the data publicly, but that would undermine the integrity and transparency of the system in a bad way, but in the future it may be possible to improve the situation without sacrificing anything through the use of zero-knowledge proofs.
