# setup-fedora

Setting up Fedora:

  1. Secure DNS (dns.conf files for systemd-resolved and NetworkManager)
  2. VPN (see below)
  3. TODO: Dynamic swap by Swapspace?

VPN:

  1. Maybe use "Official WARP Desktop Client"?
  2. Download wgcf
  3. Do "wgcf register"
  4. Do "wgcf generate"
  5. Do "nmcli connection import type wireguard file ./wgcf-profile.conf"
  6. If not working - change endpoint to IP from "WARP Ingress IP"
