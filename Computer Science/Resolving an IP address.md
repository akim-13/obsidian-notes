# Resolving an IP address
%% img for slide 14 %%
1. The client sends a DNS query for the requested domain to its specified DNS
   server.
2. If the DNS server doesn't have a record for that domain, it:
 - Either recursively handles the requiest so that it can eventually deliver
   an IP Address.
 - Or refers to a DNS server authorities for example, .uk and follow this, and
   subsequent referrals, to successively lower-level DNS servers.
