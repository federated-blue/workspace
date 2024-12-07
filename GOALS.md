# Goals of the project

WORK IN PROGRESS: it is vaguely formulated and will get updated as we go.

Overarching motive is creating a fully federated Bluesky software distribution.
What "federated" means exactly has become a bit blurry, so here are a few more
specific criteria:

1) autonomy - if the rest of the Universe implodes, users of your instance
  should still be able to communicate between them w/o issues, as well as with
  users of any other instance that is still alive and reachable.
2) scaling - amount of resources you'd need to run it should primarily depend
  on the number of users you have and their activity. In particular, a
  single-user instance should not require to be scaled up linearly with the
  size of the overall network.
3) interoperability - users should be able, in principle, to communicate with
  any other Bluesky user. As a temporary hack, until the required protocols get
  a widespread adoption, we may end up running community services that would
  implement federation on behalf of other instances. But the end goal is to turn
  them down and have instances talk directly to each other.
4) preserving UX - users' experience should be as close to https://bsky.app as
  possible. It will be impossible in some cases, then reasonable tradeoffs
  should be taken, while paying attention to how exactly they'd affect what
  users see and can do.


## Challenges

We already know that ActivityPub/Mastodon federation model has severe scaling
issues. Our work has a good chance of sharing them too, despite of how hard
we'll try to avoid it. For that reason we must be ready to scrape our first
attempt and make non-backwards-compatible changes to achieve better results.
