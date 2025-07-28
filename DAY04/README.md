## What is a Computer Network?
A computer network connects multiple devices to share data and resources. Examples include:

-**LAN (Local Area Network)** – Within a building.

-**WAN (Wide Area Network)** – Spanning across cities or regions.

-**Internet** – The vast global network linking everything.

 ##Why Subnetting is Useful
A subnet divides a large network into smaller, easier-to-manage sections.

Helps separate and organize devices.

Allows communication within the group.

Improves both security and performance.

## Understanding IP Addresses
Every device on a network has a unique IP address.

IPv4 → Shorter format, widely used: 192.168.0.1

IPv6 → Longer format, designed for the future: 2001:db8::1
 ##What’s a MAC Address?
A MAC address is a hardware-based unique ID assigned to network devices.

Example: AA:BB:CC:DD:EE:FF

It’s built into the device and generally doesn’t change.

 ##IPv4 vs IPv6
| Key Difference | IPv4                    | IPv6                              |
|----------------|-------------------------|-----------------------------------|
| Bit Size       | 32-bit                  | 128-bit                           |
| Looks Like     | 192.168.1.1             | 2001:db8:1234::abcd               |
| Space          | Limited (~4.3B)         | Massive (virtually infinite)      |
| Security       | Add-on (IPSec optional) | Built-in IPSec                    |

 ##TCP vs UDP Comparison
| Aspect        | TCP                          | UDP                       |
|---------------|-------------------------------|----------------------------|
| Connection    | Established (3-way handshake) | No connection             |
| Reliability   | Guaranteed with ACKs          | No guarantee              |
| Speed         | Slower but reliable           | Faster, best effort       |
| Example Use   | File transfer, emails         | Gaming, video streaming   |

 ## What is Port Forwarding?
It’s a method to open a path into your local network from outside.

Example: Forwarding port 3389 lets you remotely access your home desktop.

## What is UAC (User Account Control)?
A Windows feature that blocks apps from changing system settings without approval.

The popup that asks for admin permissions? That’s UAC at work.

 ##Styles of Information Gathering
Type	Activity Nature	Common Tools
Passive	No direct interaction	WHOIS, Shodan, Google
Active	Direct probing involved	Nmap, ping, traceroute

## Why Use Nmap?
Nmap is a powerful tool for network scanning. It lets you:

Discover active devices

Scan open ports

Identify OS and running services

## How an Attack Unfolds
Victim gets a phishing email with a .zip attachment.

User opens the archive and runs an .exe file.

The file connects silently to the attacker’s system.

Attacker delivers PowerShell scripts remotely.

UAC prompts flood the screen to trick the user.

If approved, full control is lost to the attacker.

Note: Don’t run files you weren’t expecting—even from trusted contacts.
 Breaking Down an Nmap Command

| Flag       | What It Does                                                   |
|------------|----------------------------------------------------------------|
| `-Pn`      | Skip pinging – treat all hosts as live                         |
| `-A`       | Enable OS detection, version info, and traceroute              |
| `-sV`      | Shows service versions                                         |
| `-O`       | Tries to identify the OS                                       |
| `-oN`      | Saves readable output                                          |
| `--script` | Runs built-in scripts                                          |
| `-vv`      | Extra verbosity                                                |
| `-p`       | Lets you choose ports                                          |
| `-sS`      | SYN scan (quiet TCP scan)                                      |
| `-sT`      | TCP connect scan (fallback if SYN fails)                       |
