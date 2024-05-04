+++
title = "Use Cases"
draft = false
weight = 90
sort_by = "weight"
template = "page.html"

[extra]
toc = true
top = false
+++

# Use Cases

In the previous examples we talked about Cassis being used as a direct payment method between users and services, but Cassis could also be used in other ways, for example:

## A transfer network for routing payments between _ecash_ mints

Currently _ecash_ technologies like **Cashu** and **Fedimint** provide immense privacy to their users, but they rely every payment that goes to external mints to be routed _instantly_ using the Lightning Network. And that can be a problem as Lightning Network payments fail for lack of liquidity or sometimes take a long time to settle.

As these mints are very similar to traditional banks, it makes a lot of sense for them to have nightly (or weekly, monthly) settlements that are not performance-critical, so theycould route payments between them using Cassis and make sporadic settlements using Lightning.
