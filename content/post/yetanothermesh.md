---
title:       "Yet another mesh"
description: "Finally I get to sort out my wifi in my little victorian terrace"
date:        2021-10-13
image: "img/wifimesh.jpg"
tags: ["Home", "Wifi", "Tech"]
categories:  ["Tech"]
---

- Bad Wifi in the house
- Bought a ubiquiti unifi dream machine https://store.ui.com/collections/unifi-network-unifi-os-consoles/products/unifi-dream-machine
- I bought a draytek vigor 130 because you can't put the sky router into bridge mode basically although there are benefits to 


link:

https://helpforum.sky.com/t5/Broadband/Draytek-130-Modem-amp-Ubiquity-Unifi-Dream-Machine-setup/td-p/3549218


updated the UDM via unifi.ui.com to UDM
UDM 1.10.0.3686

DrayTek setup:
Remove the SkyQ hub and plug all the DSL line into the new modem. 
Power this up. 
No internet for this =>You will want to hardwire a machine into the modem and browse to the modem management interface 192.168.2.1 

http://192.168.2.1 with a username of "admin" and a password of "admin" by default.

Clicked enableMPoA & VCi changed to 101

Ok and restart

Plug an ethernet cable from the DrayTek modem into the WAN port of the Dream Machine(DM). Power up the DM.Now… at this point if you are on the latest firmware and are on the same Superfast line such as I am on in England you could stop here.

Yes? Nope didn't work at the UDM is slowly flashing blue which apparently means that the UDM is connected via bluetooth

Now going to try and access vigor in bridge mode. Bridge mode means that it is purely acting as a modem. https://www.draytek.com/support/knowledge-base/5212



and click on ‘Internet Access’ then ‘MPoA/Static Dynamic IP’ then click the ‘enable’ button. Click OK and then you may need to click OK again, bit odd as I seem to remember, the first OK kind of activates the settings then OK again to apply and restart. DrayTek’s own instructions are here: https://www.draytek.co.uk/support/guides/kb-vigor-130-bridge The modem should now reboot. You can unplug your machine from the modem and continue, we are done here.