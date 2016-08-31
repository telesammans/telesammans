# telesammans

Telesammans är en gemenskap. Tillsammans har vi ett LAN.

## Teknisk översikt för vårat LAN

Backbone i vårat LAN är ett meshnätverk över ad-hoc wifi, som använder batman-adv routing.

Vi har tre centraliserade tjänster i vårat LAN:

1. Det finns en central DHCP-server som delar ut IP-adresser inom subnätet 10.160.0.0/16.
2. Det finns en tor-proxy som tillhandahåller .onion-anslutning samt Internetanslutning över tor. DHCP-servern anger denna tor-proxy som default gateway i vårat nät.
3. Det finns en DNS-server. Om du tillhandahåller någon slags tjänst inom LAN:et så kan du registrera ett domännamn i DNS-servern. Det fungerar enligt dyndns-principen, eftersom att alla IP-nummer alltid tilldelas dynamiskt inom LANet.

För att underlätta anslutning till vårat LAN så förekommer även tradionellt konfigurerade wifi-routrar (icke-mesh) som ger en anslutning bakom NAT (IP masquerading).

## Socialt kontrakt

Vi är goda grannar i vårat LAN. Vi sätter inte lösenord på våra WiFI-nätverk. Vi delar med oss.
