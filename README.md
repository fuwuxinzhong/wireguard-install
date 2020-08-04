# WireGuard installer

<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

**This project is a bash script that aims to setup a [WireGuard](https://www.wireguard.com/) VPN on a Linux server, as easily as possible!**

WireGuard is a point-to-point VPN that can be used in different ways. Here, we mean a VPN as in: the client will forward all its traffic trough an encrypted tunnel to the server.
The server will apply NAT to the client's traffic so it will appear as if the client is browsing the web with the server's IP.

The script supports both IPv4 and IPv6. Please check the [issues](https://github.com/angristan/wireguard-install/issues) for ongoing development, bugs and planned features!

WireGuard does not fit your environment? Check out [openvpn-install](https://github.com/angristan/openvpn-install).

## Requirements

Supported distributions:

- Ubuntu >= 16.04
- Debian 10
- Fedora
- CentOS
- Arch Linux

## Usage

Download and execute the script. Answer the questions asked by the script and it will take care of the rest.

```bash
curl -O https://raw.githubusercontent.com/angristan/wireguard-install/master/wireguard-install.sh
chmod +x wireguard-install.sh
./wireguard-install.sh
```

It will install WireGuard (kernel module and tools) on the server, configure it, create a systemd service and a client configuration file.

Run the script again to add or remove clients!

## Providers

I recommend these cheap cloud providers for your VPN server:

- [Vultr](https://goo.gl/Xyd1Sc): Worldwide locations, IPv6 support, starting at \$3.50/month
- [Hetzner](https://hetzner.cloud/?ref=ywtlvZsjgeDq): Germany, IPv6, 20 TB of traffic, starting at €3/month
- [Digital Ocean](https://goo.gl/qXrNLK): Worldwide locations, IPv6 support, starting at \$5/month
- [PulseHeberg](https://goo.gl/76yqW5): France, unlimited bandwidth, starting at €3/month

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://stanislas.blog/"><img src="https://avatars1.githubusercontent.com/u/11699655?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Stanislas</b></sub></a><br /><a href="#question-angristan" title="Answering Questions">💬</a> <a href="https://github.com/angristan/wireguard-install/issues?q=author%3Aangristan" title="Bug reports">🐛</a> <a href="https://github.com/angristan/wireguard-install/commits?author=angristan" title="Code">💻</a> <a href="#infra-angristan" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-angristan" title="Maintenance">🚧</a> <a href="#projectManagement-angristan" title="Project Management">📆</a> <a href="https://github.com/angristan/wireguard-install/pulls?q=is%3Apr+reviewed-by%3Aangristan" title="Reviewed Pull Requests">👀</a></td>
    <td align="center"><a href="https://keybase.io/randomshell"><img src="https://avatars3.githubusercontent.com/u/43271778?v=4?s=100" width="100px;" alt=""/><br /><sub><b>randomshell</b></sub></a><br /><a href="#question-randomshell" title="Answering Questions">💬</a> <a href="https://github.com/angristan/wireguard-install/issues?q=author%3Arandomshell" title="Bug reports">🐛</a> <a href="https://github.com/angristan/wireguard-install/commits?author=randomshell" title="Code">💻</a> <a href="https://github.com/angristan/wireguard-install/pulls?q=is%3Apr+reviewed-by%3Arandomshell" title="Reviewed Pull Requests">👀</a></td>
    <td align="center"><a href="https://github.com/lucawen"><img src="https://avatars2.githubusercontent.com/u/1365208?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Luca Lacerda</b></sub></a><br /><a href="https://github.com/angristan/wireguard-install/commits?author=lucawen" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/robiiinos"><img src="https://avatars1.githubusercontent.com/u/16455953?v=4?s=100" width="100px;" alt=""/><br /><sub><b>D. Robin</b></sub></a><br /><a href="#infra-robiiinos" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
