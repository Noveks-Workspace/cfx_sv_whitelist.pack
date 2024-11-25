Here's the README specifically for the **Noveks Discord Whitelist Script**:

---

# 🌐 Noveks FiveM Discord Whitelist Script

**Version:** 1.2.1
**Developer:** Novek  
**Discord:** [Join Support Discord](https://discord.gg/8q8BnmgXq2)  
**Tebex Store:** [Buy Here](https://noveks-workspace.tebex.io/package/6546483)  

---

## 📄 Overview

The **Noveks Discord Whitelist Script** protects your FiveM server by ensuring only players with a specific Discord role can join. This ensures better server security and community management by linking player access to your Discord server roles.

---

## 📋 Features

- 🌐 **Discord Role-Based Access Control:**  
  Only players with a designated role in your Discord server can connect.

- 🎨 **Customizable AdaptiveCards:**  
  Displays a custom message when a player without the required role attempts to join.

- 🔗 **Seamless Discord Integration:**  
  Automatically checks players’ Discord roles using the Discord API.

- 👋 **User-Friendly Notifications:**  
  Players without the correct role receive a detailed message and a Discord invite link to obtain the role.

- ⚡ **Real-Time Role Verification:**  
  The script verifies the player’s role in real-time before allowing access.

---

## ⚙️ Installation

1. **Download the Script:**  
   Place it in your server’s **`resources`** folder.

2. **Add to `server.cfg`:**  
   Add the following line to your `server.cfg`:
   ```lua
   ensure Noveks_DiscordWhitelist
   ```

3. **Set Up Discord Bot:**  
   - Create a Discord bot and get its token.
   - Ensure the bot has permission to read member roles in your server.

---

## 🛠️ Configuration

Edit the `Noveks_CFG.lua` file with the following settings:

```lua
Noveks_CFG.Settings = {
    discord = {
        discordGuildId = YOUR_DISCORD_SERVER_ID,  -- Insert your Discord server ID
        botToken = 'YOUR_DISCORD_BOT_TOKEN'         -- Insert your Discord bot token
    },

    whitelistRole = YOUR_ROLE_ID,                 -- Insert the required Discord role ID

    lang = {
        not_whitelisted = "You are not whitelisted on ServerName.",  
        check_connection = "Make sure your Discord is linked to FiveM.",
        join_discord = "Join our Discord here: https://discord.gg/yourlink"  -- Insert your Discord invite link
    },

    card = {
        image = 'YOUR_SERVER_LOGO_URL',             -- Insert the URL to your server logo
        discordUrl = 'https://discord.gg/yourlink'  -- Insert your Discord invite link
    }
}
```

## 📢 How It Works

1. **Role Verification:**  
   When a player attempts to join your server, the script checks their linked Discord account for the required role.

2. **Access Control:**  
   - Players with the correct role are allowed to connect.  
   - Players without the role see a message with an invite link to your Discord server.

---

## 💬 Support

Need help or have questions? Join our **Support Discord**:  
[Noveks Support Discord](https://discord.gg/8q8BnmgXq2)

---

### 📑 License

This script is **not open-source** and is subject to the following terms:  

- **Usage:** Licensed for use on your own server only. Redistribution or resale is prohibited.  
- **Modifications:** You may not modify or distribute the script without explicit permission.  
- **Escrow Protection:** Usage terms follow Tebex escrow platform rules.  

---

🚀 **Secure your FiveM server with Noveks Discord Whitelist Script today!** ✨
