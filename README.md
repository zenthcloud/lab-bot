# Zenth Lab Discord Bot

The **Zenth Lab Discord Bot** is an open-source command-driven assistant that allows users to deploy, manage, and interact with cybersecurity and cloud labs directly from Discord. It integrates with the Zenth Cloud infrastructure to provision ephemeral, secure lab environments for training, pentesting, or academic purposes.

---

## ✨ Features

- 🚀 Launch cyber labs and training environments via Discord commands
- 🔒 Role-based access and user authentication
- 🧪 Integration with Zenth Cloud infrastructure (Proxmox, Docker, Kubernetes)
- ⏳ Automatic lab expiration and lifecycle control
- 📡 Real-time status updates and logs
- 🧠 Designed for education, pentesting, and research communities

---

## 💬 Available Commands

| Command | Description |
|--------|-------------|
| `/lab launch [lab_name]` | Launch a predefined lab |
| `/lab list` | List all available labs |
| `/lab status [lab_id]` | Check the status of an active lab |
| `/lab stop [lab_id]` | Stop a running lab manually |
| `/lab help` | Get help on usage |

---

## 🏗 Architecture

- **Bot Framework**: `discord.py` or `discord.js`
- **API Backend**: Connects to `zenth-cyber-orchestrator` for infrastructure provisioning
- **Cloud Providers**: Integrates with Zenth Container Server, Proxmox, Kubernetes
- **SSO & Access**: Uses Zenth SSO or Discord roles for access control
- **Monitoring**: Connected to Zenth Monitoring Server

---

## 🧰 Requirements

- Python 3.10+ or Node.js 18+
- Discord Bot Token
- Access to Zenth Cloud API
- Optional: VPN or proxy access to internal infrastructure

---

## 🚀 Getting Started

1. Clone the repository:

```bash
git clone https://github.com/zenthcloud/lab-bot.git
cd lab-bot
````

2. Set up your environment variables:

```env
DISCORD_BOT_TOKEN=your_token_here
ZENTH_API_URL=https://api.zenthcloud.com/labs
ZENTH_API_KEY=your_api_key_here
```

3. Install dependencies and run the bot:

```bash
# Node.js version
npm install
node index.js
```
---

## 📚 Use Cases

* Cybersecurity training (Kali Linux, CTFs, pentest labs)
* Educational environments for schools or universities
* Research & development on cloud security
* Discord-integrated community labs (HTB-style)

---

## 🔗 Links

* 🔗 Zenth Cloud: [Website](https://zenthcloud.com)
* 🔧 Zenth Cyber Orchestrator: `zenth-cyber-orchestrator`
* 📦 Zenth Container Server: `zenth-container-server`
* 📚 Labs and curriculum: `zenth-network-academic`

---

## 🛡 License

This project is licensed under the **AGPLv3**. See [LICENSE](./LICENSE) for details.

---

## 🤝 Contributing

We welcome community contributions! Please open issues, submit PRs, or join the discussion on [Discord](https://discord.gg/zenthcloud) or Matrix.
