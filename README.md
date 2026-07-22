#  Raspberry Pi Cybersecurity Home Lab

> A Raspberry Pi 5-based home security server integrating VPN, private DNS, firewall, and a controlled environment for attack simulation.

##  Project Objectives

- **Secure remote access** via WireGuard VPN, enabling encrypted connections from anywhere.
- **Full DNS privacy** using Pi-hole + Unbound, eliminating reliance on third-party DNS servers.
- **Perimeter security** with UFW firewall configured with a default-deny policy.
- **Isolated testing lab** for simulating DoS/DDoS attacks without affecting the home network.

##  Technologies Used

| Technology | Purpose |
|------------|---------|
| WireGuard | Modern, fast, and secure VPN |
| Pi-hole | DNS-level ad and tracker blocking |
| Unbound | Recursive DNS server for maximum privacy |
| UFW | Firewall with restrictive policy |
| DuckDNS | Free DDNS for dynamic IP addresses |
| OpenMediaVault | Network-attached storage (NAS) |

##  Network Architecture

Internet → Router (Virgin Media Hub 5) → Raspberry Pi 5 (192.168.0.224)
                                           ↓
                                      WireGuard VPN
                                           ↓
                                 Acceso remoto (móvil/laptop)
                                           ↓
                                      Pi-hole + Unbound
                                           ↓
                                      Firewall UFW
                                           ↓
                                      Red doméstica protegida

##  Current Status

- [x] WireGuard VPN operational with remote access
- [x] Pi-hole + Unbound integrated
- [x] UFW firewall configured
- [x] DuckDNS auto-updating
- [x] Isolated attack lab established

## Lessons Learned

