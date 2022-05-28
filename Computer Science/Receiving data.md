# Receiving data
At the destination, the message is passed back up through the layers.

1. The [[Link layer|link layer]] removes the MAC address form each packet and
   passes it to the [[Internet layer|internet layer]]
2. The internet layer removes the IP address from each packet and passes it to
   the [[Transport layer|transport layer]]
3. The transport layer removes the port number from each packet, reassembles
   the packets in the correct order and passed them to the 
   [[Application layer|application layer]].
4. The application layer presents the image data for the user in a browser.
