# Packet trailer
**Packet trailer** — a part of a packet which contains error checking
components that verify the data received in the payload has not been corrupted
on transfer.

Techniques such as **checksums** or Cyclical Redundancy Checks (**CRSs**) are
used to check the data by the receiving host. The same checksum is recalculated
at the destination end. If they do not match, the data has become corrupted and
is refused and a new copy is requested to be sent again.
