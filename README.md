# FakerX

<div>
  <img src="https://raw.githubusercontent.com/teaminfinitydev/teaminfinitydev/refs/heads/main/img/fakerx_banner.svg" alt="FakerX Banner">
</div>

![FakerX Logo](https://img.shields.io/badge/FakerX-v1.0.0-brightgreen)
![Paper](https://img.shields.io/badge/Paper-1.21+-blue)
![Java](https://img.shields.io/badge/Java-21-orange)
![License](https://img.shields.io/badge/License-MIT-yellow)


A lightweight Minecraft plugin for Paper 1.21+ that displays fake player counts in the server list without spawning actual entities or bots in-game.


## 📋 Table of Contents

- [Features](#-features)
- [Installation](#-installation)
- [Configuration](#-configuration)
- [Commands](#-commands)
- [Permissions](#-permissions)
- [Building from Source](#-building-from-source)
- [FAQ](#-faq)
- [Support](#-support)
- [License](#-license)

## ✨ Features

- **Fake Player Count**: Display a customizable number of fake players in the server list
- **Random Count**: Randomize the player count between minimum and maximum values on each ping
- **Real Player Integration**: Option to include actual online players in the count
- **Custom Player Names**: Display fake player names in the server hover list
- **Easy Configuration**: Simple YAML configuration with hot-reload support
- **Lightweight**: Minimal performance impact on your server
- **Paper Optimized**: Built specifically for Paper 1.21+ servers

## 📦 Installation

1. **Download** the latest release from the [Releases](https://github.com/teaminfinitydev/FakerX/releases) page
2. **Place** the `FakerX.jar` file in your server's `plugins` folder
3. **Start** your server to generate the default configuration
4. **Configure** the plugin by editing `plugins/FakerX/config.yml`
5. **Reload** the configuration with `/fakeplayers reload` or restart your server

## ⚙️ Configuration

The plugin creates a `config.yml` file in the `plugins/FakerX/` directory:

```yaml
# FakerX Configuration
# https://codenexa.online

# Enable or disable the plugin
enabled: true

# Minimum number of fake players to show
min_fake_players: 5

# Maximum number of fake players to show
max_fake_players: 20

# Whether to include real players in the count
include_real_players: true

# Whether to show fake player names in the server hover list
show_fake_names: true

# List of fake player names to display
fake_names:
  - "Notch"
  - "Herobrine"
  - "Dinnerbone"
  - "jeb_"
  - "Steve"
  - "Alex"
  - "CaptainSparklez"
  - "DreamWasTaken"
  - "Technoblade"
  - "PewDiePie"

# Messages
messages:
  reload_success: "&aFakerX configuration reloaded successfully!"
  no_permission: "&cYou don't have permission to use this command!"
  plugin_disabled: "&cFakerX is currently disabled!"
```

### Configuration Options

| Option | Type | Default | Description |
|--------|------|---------|-------------|
| `enabled` | boolean | `true` | Enable/disable the plugin |
| `min_fake_players` | integer | `5` | Minimum number of fake players |
| `max_fake_players` | integer | `20` | Maximum number of fake players |
| `include_real_players` | boolean | `true` | Add real players to the fake count |
| `show_fake_names` | boolean | `true` | Show fake names in server hover list |
| `fake_names` | list | See config | List of fake player names to display |

## 🔧 Commands

| Command | Aliases | Description | Permission |
|---------|---------|-------------|------------|
| `/fakeplayers` | `/fp`, `/fakerx` | Main plugin command | `fakerx.admin` |
| `/fakeplayers reload` | - | Reload the configuration | `fakerx.admin` |
| `/fakeplayers status` | - | Show plugin status | `fakerx.admin` |
| `/fakeplayers help` | - | Show help message | `fakerx.admin` |

## 🔐 Permissions

| Permission | Default | Description |
|------------|---------|-------------|
| `fakerx.admin` | `op` | Access to all FakerX commands |


## ❓ FAQ

**Q: Will this affect actual players joining the server?**
A: No, this only changes what appears in the server list. Real players can still join normally.

**Q: Can other plugins detect these fake players?**
A: No, the fake players only exist in the server list ping response.

**Q: Does this work with server list websites?**
A: Yes, any service that pings your server will see the fake player count.

**Q: Can I use custom skins for fake players?**
A: Currently, only names are supported. Skins are not implemented in this version.

**Q: Is this compatible with other player count plugins?**
A: It may conflict with other plugins that modify server list responses. Test compatibility carefully.

## 🐛 Known Issues

- Fake player names are limited to what the client displays (typically 12-16 players)
- Custom skins are not supported in the current version
- Some client modifications may detect discrepancies

## 🔮 Planned Features

- [ ] Custom player skins support
- [ ] Time-based player count variations
- [ ] Multiple server list profiles
- [ ] Advanced randomization patterns
- [ ] Integration with other plugins

<br/>
<div align="center">
  <img src="https://raw.githubusercontent.com/teaminfinitydev/teaminfinitydev/refs/heads/main/img/codenexa_sponsor_banner_new.svg" alt="FakerX Sponsor Banner">
</div>

## 🆘 Support

- **Issues**: Report bugs on our [GitHub Issues](https://github.com/teaminfinitydev/FakerX/issues) page
- **Documentation**: Visit our [Wiki](https://github.com/teaminfinitydev/FakerX/wiki)
- **Website**: [https://codenexa.online](https://codenexa.online)

## 📄 License

This project is licensed under the GNU GENERAL PUBLIC LICENSE - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Chamika Samaraweera**
- Website: [https://codenexa.online](https://codenexa.online)
- Website: [https://teaminfinity.pro](https://teaminfinity.pro)
- GitHub: [@teaminfinitydev](https://github.com/teaminfinitydev)

## 🙏 Acknowledgments

- Thanks to the Paper team for their excellent server software
- Inspired by the Minecraft community's need for server list customization
- Special thanks to all contributors and testers

---

**⚠️ Disclaimer**: This plugin is designed for legitimate server management purposes. Please ensure you comply with your hosting provider's terms of service and Minecraft's EULA when using this plugin.

**📝 Note**: FakerX is not affiliated with Mojang Studios or Microsoft.

