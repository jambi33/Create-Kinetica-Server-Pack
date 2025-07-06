# Create Kinetica Server Modpack Files

A comprehensive server modpack for Minecraft with performance optimizations and custom configurations.

**Required:** NeoForge 21.1.172

## How to Download

1. **Download the server files:**
   - Click the green "Code" button above
   - Select "Download ZIP"
   - Extract the ZIP file to your desired server location

2. **Alternative - Git Clone:**
   ```bash
   git clone https://github.com/jambi33/Create-Kinetica-Server-Pack.git
   ```

3. **Required additional files:**
   - Download NeoForge 21.1.172 server installer from [NeoForge Downloads](https://neoforged.net/downloads)
   - Accept the Minecraft EULA by creating `eula.txt` with `eula=true`
   - Configure your `server.properties` file (see configuration section below)

## Where to Upload

**For server hosting, upload these files to:**
- **Shared hosting providers:** Upload via FTP/SFTP to your server directory
- **VPS/Dedicated servers:** Upload to your Minecraft server folder (typically `/opt/minecraft/` or `~/minecraft/`)
- **Local hosting:** Place in your chosen server directory

**Important:** Do not upload `world/`, `logs/`, or `crash-reports/` folders if they exist locally.

## Recommended Minimum Specs

### Memory (RAM) Requirements

| Server Size | RAM | Player Count | Description |
|-------------|-----|--------------|-------------|
| **Small** | 8GB | 1-5 players | Perfect for small friend groups and testing |
| **Medium** | 16GB | 6-15 players | Ideal for medium communities and active servers |
| **Large** | 32GB | 16-30 players | Suitable for large communities and public servers |

*Note: These are minimum requirements. More RAM will improve performance, especially with chunk loading and mod processing.*

### CPU Specifications

| Performance Level | CPU Requirements | Examples |
|------------------|------------------|----------|
| **Minimum** | 4 cores, 3.0+ GHz | Intel i5-8400, AMD Ryzen 5 2600 |
| **Average** | 6-8 cores, 3.5+ GHz | Intel i7-9700K, AMD Ryzen 7 3700X |
| **Excellent** | 8+ cores, 4.0+ GHz | Intel i9-11900K, AMD Ryzen 9 5900X |

*Single-core performance is crucial for Minecraft servers. Higher clock speeds often outperform more cores.*

### Storage Requirements

- **Highly Recommended:** NVMe SSD drive
- **Minimum:** 50GB free space for world files and backups
- **Why NVMe:** Dramatically improves chunk loading, world generation, and reduces lag spikes

## Specific Configuration Changes

This modpack includes several custom configurations for improved gameplay and performance:

### Artifacts Mod Changes
- **Disabled:** Everlasting Beef/Eternal Steak drops to maintain food progression balance

### Better Days Mod Changes
- **Day Length:** Extended to 40 minutes (from default 20 minutes)
- **Night Length:** Reduced to 20 minutes (from default 10 minutes)
- **Purpose:** Provides more productive daylight hours while maintaining night cycle challenges

### Performance Optimizations

#### Distant Horizons Recommendations
For optimal server performance, consider one of these options:

1. **Remove Distant Horizons entirely** (recommended for larger servers)
2. **Reduce server properties amounts** in `DistantHorizons.toml` config file to optimize performance

#### Server Properties Optimization
Recommended settings for `server.properties`:
```properties
view-distance=8
simulation-distance=6
max-tick-time=60000
entity-activation-range=32
```

### Custom Mods Included

#### Villager AI Optimizer
- **Purpose:** Improves server performance by disabling villager AI and pathfinding
- **Conditions:** AI disabled when confined to a single block area, or nametag "noai" is used on villager
- **Benefits:** Reduces server lag in areas with many villagers, like trading halls
- **GitHub Repository:** Link coming soon

### Communication Mods Configuration

#### Simple Discord Link Bot
- **Purpose:** Links your Minecraft server chat with a Discord channel
- **Setup Required:** Configure with your own Discord server settings
- **Alternative:** If you don't have a Discord server, this mod can be ignored or removed
- **Configuration Guide:** [Setup Documentation](https://sdlink.fdd-docs.com/)

#### Simple Voice Chat
- **Purpose:** Enables proximity voice chat between players on the server
- **Setup Required:** Open port 24454 on your server firewall
- **Configuration Guide:** [Server Setup Wiki](https://modrepo.de/minecraft/voicechat/wiki/server_setup)
- **Benefits:** Enhances multiplayer communication and immersion

## Setup Instructions

1. **Install NeoForge 21.1.172** on your server
2. **Copy all mod files** to the `mods/` folder
3. **Copy configuration files** to the `config/` folder
4. **Create server.properties** with your desired settings
5. **Accept EULA** by creating `eula.txt` with `eula=true`
6. **Start your server** and enjoy!

## Support

For issues, questions, or suggestions:
- Open an issue on this GitHub repository
- Check the mod compatibility list in the `mods/` folder
- Ensure you're using the correct NeoForge version

## License

This modpack is provided as-is. Individual mods retain their respective licenses. Please respect mod authors' terms of use.

---

*Happy crafting with Kinetica Server Modpack!*