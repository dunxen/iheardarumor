# iheardarumor

This toy Lightning Network project is just meant for educational purposes. It's a dumb node that just participates in the P2P gossip protocol. So the only three messages that are of interest to it are:

  - `node_announcement`
  - `channel_announcement`
  - `channel_update`

The `announcement_signatures` message plays no role here as the node does not accept channels or participate in the rest of the protocol.
In essence we're just implementing everything in [BOLT 7](https://github.com/lightning/bolts/blob/master/07-routing-gossip.md#the-announcement_signatures-message) except for anything to do with `announcement_signatures`.
