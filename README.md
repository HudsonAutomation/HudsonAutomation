# Hudson Automation

**More calls. Less chasing.** Missed-call text-back, AI voice agents, review requests and websites for local businesses in Humboldt County, CA.

🌐 [hudsonautomation.netlify.app](https://hudsonautomation.netlify.app)

---

## 🛠️ Build log

### Friday, November 13, 2026: home lab infrastructure day

- 🔐 **Private mesh network:** added two more Linux machines to a Tailscale tailnet, so every machine connects securely with no ports opened to the internet.
- 🛡️ **Network-wide ad and tracker blocking:** Pi-hole, running on an old 32-bit laptop brought back to life with antiX Linux, is now the DNS resolver for every device on the tailnet, phone included.
- 🎵 **Discord music bot moved to low-power hardware:** the CupboardLabs music bot now runs on that same Linux box, starts automatically on boot, and the old Windows auto-start was retired.
- 🐛 **Silent voice audio fixed:** traced it to a breaking release of the `davey` DAVE voice-encryption library (0.2.0) that discord.py 2.7.1 doesn't support yet. Pinning `davey>=0.1.7,<0.2` brought the audio back.
- 📈 **Monitoring (in progress):** staging an Uptime Kuma status dashboard and a backup Pi-hole on a third machine.
