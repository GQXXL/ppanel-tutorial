# Clash Verge for macOS

## 📥 Download Links

- **Clash Verge Apple Silicon (M series)**: [Click to download](https://gh.xxooo.cf/https://github.com/clash-verge-rev/clash-verge-rev/releases/download/v2.4.7/Clash.Verge_2.4.7_aarch64.dmg)
- **Clash Verge Intel**: [Click to download](https://gh.xxooo.cf/https://github.com/clash-verge-rev/clash-verge-rev/releases/download/v2.4.7/Clash.Verge_2.4.7_x64.dmg)
- **Official latest installer**: [Go to download](https://github.com/clash-verge-rev/clash-verge-rev/releases/)

## ⚠️ macOS Security Settings

### 🛡️ Fix common security warnings

You may see warnings on first launch:

- "Developer cannot be verified"
- "App is damaged"
- "From an unidentified developer"

#### 🔧 Steps

1. Install from DMG and try opening the app first.
2. Go to **System Settings → Privacy & Security**.
3. In **General**, click **Open Anyway**.
4. Confirm opening the app.

If needed, use Terminal:

```bash
sudo xattr -r -d com.apple.quarantine /Applications/Clash\ Verge.app
```

> ⚠️ Security tip: only run commands you understand.

---

## 🚀 Configuration Tutorial

### 📋 Before you start

- ✅ Clash Verge installed successfully
- ✅ Valid subscription URL or config file
- ✅ macOS security warning resolved
- ✅ Network is working

### 🛠️ Configuration steps

1. Open Clash Verge.
2. Go to **Profiles / Configuration**.
3. Click **New / +**, choose **Subscription**.
4. Enter name + subscription URL and save.
5. Update subscription regularly.

---

## 🎛️ Advanced Features

### 📊 Traffic monitoring

- Real-time upload/download speed
- Connection details
- Traffic by app

### 🎯 Policy setup

- Auto-select best node by latency
- Manual node selection
- Failover and load balancing

### 🎨 UI customization

- Light/Dark theme
- Language options
- Layout preferences

---

## ⚙️ System Integration

### 🌐 System proxy

- HTTP proxy
- SOCKS5 proxy
- PAC mode
- TUN mode (extra setup may be required)

### 🔧 Auto start

- Launch at startup
- Minimize to tray/menu bar
- Tray status icon
- Global shortcuts

---

## ❓ FAQ

### 🔧 Installation issues

**Q: App cannot be opened and says damaged?**

A:
- Use **Privacy & Security → Open Anyway**
- Or run:
  `sudo xattr -r -d com.apple.quarantine /Applications/Clash\ Verge.app`

**Q: Which version should I download?**

A:
- Apple Silicon (M1/M2/M3): aarch64
- Intel Macs: x64

### 🌐 Connection issues

**Q: Imported config but cannot connect?**

A:
- Check subscription URL validity
- Check network connection
- Try switching nodes
- Check app logs

**Q: Connected but no internet?**

A:
- Verify system proxy settings
- Check firewall restrictions
- Try another mode
- Restart network service

---

## 💡 Best Practices

### ⚡ Performance

1. Use nearby nodes
2. Keep rules simple and clean
3. Update subscriptions daily
4. Disable unused features

### 🛡️ Security

1. Keep app updated
2. Backup configs regularly
3. Grant only necessary permissions
4. Use trusted subscription sources
