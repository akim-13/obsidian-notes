# Packet header
**Packer header** -- the part of a packet which contains the recipient's
address so that it can be directed appropriately across the network.

The address of the sender is also included so that replies can be sent
appropriately. 

The packer number and overall number of packets in the transmission is attached
to assist in reassembling the data.

The Time To Live (**TTL**) or hop limits is also included.
