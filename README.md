<div id="top" align="center">

<!-- Logo -->
<a href="https://github.com/franckferman/Bikochu">
  <img src="https://raw.githubusercontent.com/franckferman/Bikochu/refs/heads/stable/docs/github/graphical_resources/Logo-without_background-Bikochu.png" alt="Bikochu Logo without background" width="auto" height="auto">
</a>

<!-- Title & Tagline -->
<h3 align="center">🪲 Bikōchū (微香虫)</h3>
<p align="center">
    <em>DIY Self-Hosted - Shodan × Nessus × Metasploit, in one offensive platform.</em>
    <br>
    Remember, track, uncover: the shinobi way of Bikōchū's scanning.
</p>

</div>

## About

**Bikōchū** (微香虫) is a DIY offensive, fully self-hosted recon platform - built for deep Internet-wide reconnaissance, proof-based vulnerability hunting, and governed exploitation.

> Inspired by the "scent bug" from Naruto, Bikōchū's mission is simple: sniff out what others don't see - exposed services, weak configurations, vulnerabilities, and exploitation vectors - on a massive scale.

> Bikōchū is not just a port scanner. It's a full offensive recon-to-exploitation engine for security researchers, red teams, and anyone who thinks like an attacker.

### Origin & Vision

Bikōchū was originally inspired by a **Military Interest Intelligence** project (RIM - **Renseignement d'Intérêt Militaire**), focused on reconnaissance, large-scale data aggregation, and target analysis.

It has since grown into something far larger - and far more capable - than that first idea.

**Status: closed-source & private, for now.** Bikōchū has become powerful enough that shipping it openly, as-is, would be irresponsible. Before any public release we're deliberately taking the time to define its scope, its limits, and its guardrails. The project is under active development; whether an open-source edition ever ships - and how it would sit alongside premium offerings - is still an open question.

### Architecture

Bikōchū is built where each layer earns its language:

- **Python** - backend, scan orchestration, detection plugins, integrations
- **TypeScript / React** - the web console (dashboard, 3D globe, live scans, analytics)
- **Shell** - zero-dependency agent bootstrap

By design it's architected to grow into a multi-language framework - a static **Go** agent and a **Rust** hot-path parser are on the roadmap, each chosen for what it does best.

### Capabilities

**Reconnaissance & scanning**
- Internet-wide scanning (nmap + masscan) - by IP, CIDR, ASN or country
- Service fingerprinting, banner grabbing, TLS/JARM, GeoIP (3-axis), ASN, reverse DNS
- Shodan-style searchable database - every result indexed and queryable
- Distributed scanning across multiple agents

**Vulnerability detection - proof-based**
- CPE to NVD matching against the full CVE database
- Hundreds of custom plugins with a CONFIRMED-vs-POTENTIAL, zero-false-positive discipline
- Integrated Nuclei + a generic web-attack toolbox (XSS / SQLi / SSTI / XXE / LFI)

**Exploitation & C2 - governed**
- Autopwn handoff from a confirmed finding to a provenanced C2 session - MOCK by default, nothing fires on its own
- Metasploit integration, payload catalog, listeners, mission & tasking model

**Intelligence & OSINT**
- Passive DNS / TLS / HTTP, network-flow analysis, subdomain enumeration
- CVE / EPSS / KEV / Exploit-DB feeds, multi-engine dorking

**Platform**
- Web console with 3D globe, maps and analytics
- Native AI assistant + MCP server (drive the data from LLM agents)
- 100% self-hosted - no SaaS, no per-IP cap

## Disclaimer

Bikōchū is intended for authorized security research and testing only. Use it exclusively against systems you own or have explicit written permission to assess. You alone are responsible for any use of this tool.

## License

Licensed under the GNU Affero General Public License v3.0. See [LICENSE](https://github.com/franckferman/Bikochu/blob/stable/LICENSE) for full terms.

## Contact

[![ProtonMail][protonmail-shield]](mailto:contact@franckferman.fr)
[![LinkedIn][linkedin-shield]](https://www.linkedin.com/in/franckferman)
[![Twitter][twitter-shield]](https://www.twitter.com/franckferman)

<!-- MARKDOWN LINKS & IMAGES -->
[protonmail-shield]: https://img.shields.io/badge/ProtonMail-8B89CC?style=for-the-badge&logo=protonmail&logoColor=blueviolet
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=blue
[twitter-shield]: https://img.shields.io/badge/-Twitter-black.svg?style=for-the-badge&logo=twitter&colorB=blue
