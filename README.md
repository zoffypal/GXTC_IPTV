Self-hosted GX Telecom IPTV.  
Need an IPTV account to PPPoE, udpxy or msd_lite forwards IPTV multicast to LAN.  
IPTV account and password can be found in Telecom TV box sets settings(default settings password is 10000), IPTV account format is like iptvxxxxxx@iptv.gx, default password is 111111.  
Create a new PPPoE interface with IPTV account, and set the port to ethx that connected to ONU iTV port, and the metri must above 10 in case default internet route via IPTV interface.  
If your router only had 1 port, set the IPTV interface on vlan43. In ONU, set the IPTV to same vlan.  
IPTV interface should get an IP like 10.x.x.x if PPPoE successful.  
Use udpxy or msd_lite forwards IPTV multicast to LAN, source is pppoe-iptv.  
Replace address to your router address and udpxy port in m3u file.  
Enjoy your TV with m3u player.
