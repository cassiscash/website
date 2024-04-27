+++
title = "A protocol for small transfers"

[extra]
lead = '<b>Cassis</b> is a way to leverage (and enhance) <b>social trust</b> in order to send satoshis without incurring in complicated and costly blockchain operations.'
button_url = "/how-it-works/"
button_text = "Learn"
meta = "Beware: <i>trust</i> is involved."

# Menu items
[[extra.menu.main]]
name = "How it works"
section = "how"
url = "/how-it-works/introduction"
weight = 10

[[extra.menu.main]]
name = "Use cases"
section = "use"
url = "/use-cases/introduction"
weight = 15

[[extra.menu.main]]
name = "Blog"
section = "blog"
url = "/blog/"
weight = 20

[[extra.list]]
title = "Simple"
content = "Cassis works in a traditional client-server topology, and only touches Bitcoin indirectly, therefore it is very easy to reason about and to implement wallets that talk to it."

[[extra.list]]
title = "Cheap"
content = "Because it never touches the blockchain, transfer made through Cassis can be many orders of magnitude cheaper than other methods of making Bitcoin payments."

[[extra.list]]
title = "Fast"
content = "A Cassis Registry creates atomic transfers using pre-authorized scopes from participants. It's a fast operation with no communication overhead that takes less than a second."

[[extra.list]]
title = "Compatible"
content = "Transfers can be made conditional using a <i>hash-timelocked</i>-like scheme, so they can interface with the Lightning Network and other Bitcoin-native protocols atomically."

[[extra.list]]
title = "Social"
content = "Cassis relies on <i>friend-to-friend</i> trust networks, so it in some ways it can also strenghten trust ties and grow communities of Bitcoiners, which is always good."

[[extra.list]]
title = "Micropayments"
content = "Since Cassis transfers are not ever expected to be settled individually, they can be very small and thus power all types of commerce and online use-cases."

+++
