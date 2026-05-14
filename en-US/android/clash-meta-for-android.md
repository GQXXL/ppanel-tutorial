### 🛠️ Installation Steps

1. **Download Application**
   - Choose any download link above
   - Download `cmfa-2.11.6-alpha-universal-release.apk`

2. **Allow Installation**
   - Settings → Security → Enable "Unknown Sources"
   - Or select "Allow this installation" when prompted

3. **Complete Installation**
   - Tap the APK file to start installation
   - Follow prompts to complete the installation process

---

## 🚀 Usage Tutorial

### 📋 Configuration Steps

#### 🔥 Step Overview

1. **📱 Launch Application** - Open Clash Meta for Android
2. **⚙️ Import Configuration** - Add subscription links or configuration files
3. **🌐 Select Nodes** - Choose servers from the node list
4. **🚀 Enable Proxy** - Start the proxy service
5. **✅ Verify Connection** - Confirm proxy functionality is working

### 🎯 Detailed Operation

#### 🌟 Step 1: Application Launch

Open the installed Clash Meta and enter the main interface:

![Application Launch Interface](clash-meta-for-Android-01.png)

> 💡 First launch will request network permissions, please tap "Allow"

#### ⚙️ Step 2: Configuration Management

Tap the "Configuration" tab to enter the configuration management page:

![Configuration Management Page](clash-meta-for-Android-02.jpg)

#### 📥 Step 3: Import Configuration

Tap the "+" button in the top right corner and select import method:

![Import Configuration Options](clash-meta-for-Android-03.jpg)

#### 📝 Step 4: Configuration Information

Enter configuration information (subscription link or configuration file):

![Configuration Information Entry](clash-meta-for-Android-04.jpg)

#### ⏳ Step 5: Wait for Loading

After importing configuration, wait for node information to load completely:

![Configuration Loading Process](clash-meta-for-Android-05.jpg)

#### 🌐 Step 6: Select Nodes

Choose appropriate servers from the node list:

![Node Selection Interface](clash-meta-for-Android-06.jpg)

#### ✅ Step 7: Confirm Configuration

Review configuration information and save after confirming it's correct:

![Configuration Confirmation Screen](clash-meta-for-Android-07.jpg)

#### 🚀 Step 8: Start Service

Return to the main interface and enable the proxy service:

![Connection Status Display](clash-meta-for-Android-08.jpg)

---

## 🎛️ Advanced Features

### 📊 Rule Management

#### 🎯 Traffic Routing Rules

- **Domain Rules**: Smart traffic splitting based on domain names
- **IP Rules**: Precise traffic routing based on IP addresses
- **GeoIP Rules**: Automatic routing based on geographical location
- **Custom Rules**: Support for user-defined routing rules

#### 📋 Rule Configuration Examples

```yaml
# Domain-based rules
rules:
  - DOMAIN-SUFFIX,google.com,PROXY
  - DOMAIN,www.google.com,PROXY
  - DOMAIN-KEYWORD,google,PROXY

# IP-based rules
  - IP-CIDR,192.168.0.0/16,DIRECT
  - IP-CIDR,10.0.0.0/8,DIRECT

# GeoIP rules
  - GEOIP,CN,DIRECT
  - GEOIP,US,PROXY

# Default rule
  - MATCH,PROXY
```

### 🔄 Policy Group Configuration

#### 🎛️ Group Types

- **Auto Select**: Automatically choose the optimal node based on latency
- **Load Balance**: Evenly distribute traffic across multiple nodes
- **Fallback**: Automatically switch to backup nodes when primary fails
- **Manual Select**: User manually specifies which node to use

#### ⚙️ Configuration Examples

```yaml
proxy-groups:
  - name: "Auto"
    type: url-test
    proxies:
      - "Server1"
      - "Server2"
    url: 'http://www.gstatic.com/generate_204'
    interval: 300

  - name: "LoadBalance"
    type: load-balance
    proxies:
      - "Server1"
      - "Server2"
    url: 'http://www.gstatic.com/generate_204'
    interval: 300
```

### 📈 Monitoring & Statistics

#### 📊 Real-time Monitoring

- **Live Traffic**: Display current upload/download speeds
- **Connection Info**: View active connection details
- **Log Records**: Detailed runtime log information
- **Rule Matching**: Show rule hit situations

#### 📈 Performance Metrics

| Metric | Description | Update Frequency |
|--------|-------------|------------------|
| 🚀 **Speed** | Current transfer rates | Real-time |
| 📊 **Traffic** | Total data consumed | Continuous |
| 🔗 **Connections** | Active connection count | Real-time |
| ⏱️ **Latency** | Response time to servers | Periodic |

---

## 🔧 Advanced Configuration

### 🌐 DNS Configuration

```yaml
dns:
  enable: true
  listen: 0.0.0.0:53
  ipv6: false
  default-nameserver:
    - 223.5.5.5
    - 8.8.8.8
  enhanced-mode: fake-ip
  fake-ip-range: 198.18.0.1/16
  nameserver:
    - https://doh.pub/dns-query
    - https://dns.alidns.com/dns-query
```

### 🎯 Custom Rules

```yaml
# Custom rule examples
rules:
  # Streaming services
  - DOMAIN-SUFFIX,netflix.com,Streaming
  - DOMAIN-SUFFIX,hulu.com,Streaming
  - DOMAIN-SUFFIX,disney.com,Streaming

  # Social media
  - DOMAIN-SUFFIX,twitter.com,Social
  - DOMAIN-SUFFIX,facebook.com,Social
  - DOMAIN-SUFFIX,instagram.com,Social

  # Gaming
  - DOMAIN-SUFFIX,steam.com,Gaming
  - DOMAIN-SUFFIX,epicgames.com,Gaming

  # Ad blocking
  - DOMAIN-SUFFIX,googleads.com,REJECT
  - DOMAIN-SUFFIX,doubleclick.net,REJECT
```

---

## ⚠️ Important Notes

### 🛡️ Security Reminders

- **Configuration Sources**: Only use trusted configuration providers
- **Permission Management**: Grant necessary permissions reasonably
- **Regular Updates**: Update to the latest version promptly
- **Backup Configurations**: Regularly backup important configuration files

### 🔧 Compatibility

- **System Version**: Ensure Android version meets requirements
- **Hardware Architecture**: Download the appropriate architecture package
- **Network Environment**: Some networks may restrict proxy functionality

---

## ❓ Frequently Asked Questions

### 🔧 Technical Support

**Q: Unable to import configuration?**

A: Please check:

- ✅ Subscription link is correct
- ✅ Network connection is normal
- ✅ Configuration format is compatible
- ✅ No firewall blocking access

**Q: Connected but can't access internet?**

A: Troubleshooting suggestions:

- 🔄 Check if nodes are available
- 📱 Confirm VPN permissions are granted
- 🌐 Try switching to different nodes
- 🛡️ Verify DNS settings

**Q: App crashes or freezes?**

A: Solutions:

- 🔄 Restart app or device
- 🗑️ Clear app cache and data
- 📊 Check system resource usage
- 📱 Update to latest version

### 🌐 Network Issues

**Q: Slow connection speeds?**

A: Optimization tips:

- 📍 Choose servers closer to your location
- ⏰ Test at different times of day
- 🔧 Try different protocols
- 📊 Use built-in speed test

**Q: Frequent disconnections?**

A: Stability improvements:

- 🔄 Enable auto-reconnect
- 🛡️ Check battery optimization settings
- 📶 Verify network stability
- ⚙️ Adjust keep-alive settings

### ⚙️ Configuration Issues

**Q: Rules not working properly?**

A: Check points:

- 📋 Verify rule syntax is correct
- 🎯 Check rule priority order
- 🔍 Review rule matching logs
- 🔄 Restart after rule changes

---
