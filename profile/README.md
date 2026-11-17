<div align="center">

<img src="https://avatars.githubusercontent.com/u/270918707?s=200&v=4" width="96" alt="NSL.SH logo"/>

# NSL.SH

**Put your home server online, securely, in one click.**

Free and open-source domain routing for self-hosted apps.
Automatic HTTPS subdomains, no static IP, no port forwarding, no router setup.

[Website](https://nsl.sh) · [Get started](https://github.com/NSL-SH/mesh-router-root) · [Contact](mailto:contact@nsl.sh)

</div>

---

## What NSL.SH does

You run apps at home (on a NAS, a mini PC, a Raspberry Pi). Making them reachable from the internet usually means buying a static IP, opening ports on your router and managing SSL certificates by hand.

NSL.SH handles all of that for you:

- **Automatic HTTPS addresses** for every app, like `photos.yourname.nsl.sh`
- **Works behind any connection**: no static IP, no port forwarding, works behind CGNAT (the shared IP setup many ISPs use)
- **Encrypted tunnels** using WireGuard when a direct connection is not possible
- **Built for Docker**: apps are discovered and routed automatically
- **Free and open source** under the MIT license

## How it fits together

| Component | Role |
|---|---|
| [mesh-router-root](https://github.com/NSL-SH/mesh-router-root) | Start here. Entry point of the NSL.SH ecosystem |
| [mesh-router-agent](https://github.com/NSL-SH/mesh-router-agent) | Runs on your server and registers your apps |
| [mesh-router-tunnel](https://github.com/NSL-SH/mesh-router-tunnel) | WireGuard tunnel that routes traffic to your containers |
| [mesh-router-gateway](https://github.com/NSL-SH/mesh-router-gateway) | Public entry point that forwards requests to your server |
| [mesh-router-backend](https://github.com/NSL-SH/mesh-router-backend) | API for domain management |
| [mesh-router-nameserver](https://github.com/NSL-SH/mesh-router-nameserver) | DNS server for nsl.sh domains |
| [mesh-router-caddy](https://github.com/NSL-SH/mesh-router-caddy) | Web server that serves your apps over HTTPS |

## Self-hosting tools

| Project | What it is |
|---|---|
| [Maison](https://github.com/NSL-SH/Maison) | Dashboard for your self-hosted Docker apps, with a CasaOS-compatible App Store |
| [AppShield](https://github.com/NSL-SH/AppShield) | Lightweight login gate for any app: password, API token or SSO |
| [files](https://github.com/NSL-SH/files) | Web file manager with resumable uploads, previews and text editing |

## Contributing

Issues and pull requests are welcome on every repository.
Found a security problem? Please email **contact@nsl.sh** instead of opening a public issue.

## Who is behind it

NSL.SH is built by [Aptero](https://aptero.co), the team behind [Yundera](https://yundera.com), the managed personal cloud server.
