# VPN Server Lists

## Lists

* NordVPN
* ProtonVPN

## TODO

* openproxylist[.]com/openvpn/
* surfshark[.]com
* expressvpn[.]com
* cyberghostvpn[.]com
* norton[.]com

## But Why?

Occasionally, you may find yourself conducting an investigation into authorized users accessing corporate resources from mobile devices. Sometimes, these users utilize consumer VPN services, which inherently is not problematic but complicates investigations when alerts indicate resource access from unusual locations.

When confronted with such detections, many investigators rely on ASN data as a quick initial reference. However, VPN providers often mask their identities behind third-party infrastructure, making it challenging to verify whether an IP address genuinely belongs to a VPN provider.

In my research, I found that there isn't a comprehensive, regularly updated source to confirm VPN associated IP addresses reliably. While some efforts exist to maintain such lists, none seemed sufficiently robust or current based on extensive searches.

To address this gap, I am publishing this repository, aiming to create a continuously updated resource. Additionally, I have established an API endpoint to facilitate real-time access to this data, with plans to expand coverage to additional services in the future.


## API Endpoints

### NordVPN
```sh
curl https://vpnserverlist.azurewebsites.net/api/nordservers --output nord.json
```

### ProtonVPN
```sh
curl https://vpnserverlist.azurewebsites.net/api/protonservers --output proton.json
```