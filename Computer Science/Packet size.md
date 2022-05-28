# Packet size
Packets are deliberately kept *small* to ensure that individual packets do not
take excessive time to transfer preventing other packets from moving.

However, they should *not* be *too small* as the additional data added makes data
transfer inefficient as unnecessary headers and trailers would be required each
time.

The ideal size is between 500 and 1500 bytes.
