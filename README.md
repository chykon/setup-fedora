# setup-fedora

Setting up Fedora:

  1. Secure DNS (dns.conf files for systemd-resolved and NetworkManager)
  2. VPN (see below)
  3. Dynamic swap (see below)

VPN:

  1. Maybe use "Official WARP Desktop Client"?
  2. Download wgcf
  3. Do "wgcf register"
  4. Do "wgcf generate"
  5. Do "nmcli connection import type wireguard file ./wgcf-profile.conf"
  6. If not working - change endpoint to IP from "WARP Ingress IP"

Dynamic swap:

  1. Download swapspace
  2. Do "./configure"
  3. Do "make"
  4. Do "make install"
  5. Do "cp swapspace.service /etc/systemd/system/"
  6. Do "systemctl enable swapspace"
  7. Do "systemctl start swapspace"
