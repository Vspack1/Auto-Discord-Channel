# Auto-Discord-Channel
I'm tired for create so many server so I make this tool.

# 🚀 Discord Server Auto Setup Tool

**Tự động tạo và cấu hình Discord server với đầy đủ tính năng chỉ trong vài phút!**

![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)

## 📋 Mục lục

- [✨ Tính năng](#-tính-năng)
- [🚀 Quick Start](#-quick-start)
- [🔧 Cài đặt](#-cài-đặt)
- [📖 Hướng dẫn sử dụng](#-hướng-dẫn-sử-dụng)
- [⚙️ Cấu hình](#️-cấu-hình)
- [🛡️ Bảo mật](#️-bảo-mật)
- [❓ FAQ](#-faq)
- [🐛 Bug Reports](#-bug-reports)

## ✨ Tính năng

### 🎯 **Auto Setup chính**
- ✅ **Tự động tạo Roles** với màu sắc và permissions chuẩn
- 📁 **Tạo Categories và Channels** theo template
- 🔒 **Setup Permissions** cho từng nhóm user
- 🤖 **Bot Channels** tự động cho từng bot
- 🔐 **Verification System** với reaction roles
- 🎁 **Giveaway Channels** và roles ping
- 🛡️ **Staff Private Area** bảo mật
- 🔞 **NSFW Channels** (tùy chọn)

### ⚡ **Quick Templates**
- 🎮 **Gaming Community** - Server game với voice channels, bot commands
- 💬 **General Community** - Cộng đồng giao lưu cơ bản  
- 📚 **Study Group** - Server học tập với homework help
- 💼 **Business** - Server doanh nghiệp với meeting rooms
- 🎨 **Creative Hub** - Server sáng tạo với showcase channels

### 🛠️ **Tính năng nâng cao**
- 📊 **Real-time Progress** với logs chi tiết
- 💾 **Backup/Export** cấu trúc server
- 🔄 **Rate Limiting** tự động xử lý Discord limits
- ⚡ **One-click Setup** cho từng loại server
- 🎨 **Custom Channels** thêm channels tùy ý

## 🚀 Quick Start

### Bước 1: Mở tool
```bash
# Chỉ cần mở file HTML trong browser
open discord-auto-setup.html
```

### Bước 2: Lấy Discord Token
1. Mở [Discord Web](https://discord.com/app)
2. Nhấn `F12` → Tab `Application`
3. `Storage` → `Local Storage` → `https://discord.com`
4. Tìm key `"token"` và copy value (bỏ dấu ngoặc kép)

### Bước 3: Setup Server
1. Paste token vào tool
2. Chọn server cần setup
3. Chọn template và tính năng
4. Click **"🚀 Bắt đầu Auto Setup"**
5. Đợi tool tự động tạo mọi thứ!

## 🔧 Cài đặt

### 📋 Yêu cầu
- **Browser:** Chrome, Firefox, Safari, Edge (modern browsers)
- **Discord Account** với quyền Administrator trên server
- **Internet Connection** để gọi Discord API

### 📥 Download
```bash
# Clone repository
git clone https://github.com/your-repo/discord-auto-setup
cd discord-auto-setup

# Hoặc download trực tiếp file HTML
wget https://your-link/discord-auto-setup.html
```

### 🖥️ Chạy local
```bash
# Chỉ cần mở file HTML
open discord-auto-setup.html

# Hoặc dùng local server
python -m http.server 8000
# Mở http://localhost:8000
```

## 📖 Hướng dẫn sử dụng

### 🔑 **Lấy Discord User Token**

**⚠️ CẢNH BÁO:** User Token rất quan trọng, không chia sẻ với ai!

**Cách 1: Discord Web**
```javascript
// Mở Console (F12) trên discord.com và chạy:
(webpackChunkdiscord_app.push([[''],{},e=>{m=[];for(let c in e.c)m.push(e.c[c])}]),m).find(m=>m?.exports?.default?.getToken!==void 0).exports.default.getToken()
```

**Cách 2: Manual**
1. Mở Discord Web → F12
2. Application → Storage → Local Storage
3. `https://discord.com` → tìm `"token"`
4. Copy value (bỏ dấu ngoặc kép)

### 🎯 **Chọn Template**

| Template | Phù hợp cho | Tính năng |
|----------|-------------|-----------|
| 🎮 **Gaming** | Game thủ, esports | Voice channels, bot commands, events |
| 💬 **Community** | Cộng đồng chung | Chat rooms, media sharing |
| 📚 **Study** | Học tập, giáo dục | Homework help, study groups |
| 💼 **Business** | Doanh nghiệp | Meeting rooms, project updates |
| 🎨 **Creative** | Nghệ thuật, sáng tạo | Showcase, collaboration |

### 🎛️ **Cấu hình tính năng**

#### 🔐 **Verification System**
- Tạo channel `#verification`
- Setup reaction roles
- Auto-assign "Verified" role
- Chặn unverified users khỏi server chính

#### 🎁 **Giveaway System**
- Tạo category "GIVEAWAY & EVENTS"
- Channels: `#giveaways`, `#event-chat`
- Role ping cho giveaway participants
- Ready cho GiveawayBot, Carl-bot

#### 🛡️ **Staff Private Area**
- Category hoàn toàn private
- Channels: owner-only, admin-chat, mod-chat, staff-general, reports-logs
- Permissions chặt chẽ theo hierarchy

#### 🤖 **Bot Integration**
- Tự động tạo channels cho từng bot
- Naming convention: `#botname-commands`
- Category riêng cho tất cả bot channels
- Support: MEE6, Carl-bot, Dyno, Mudae, v.v.

## ⚙️ Cấu hình

### 🎭 **Default Roles**

| Role | Color | Permissions | Mô tả |
|------|-------|-------------|-------|
| 👑 Owner | 🔴 Red | Administrator | Chủ server |
| ⚡ Administrator | 🟠 Orange | Administrator | Admin team |
| 🛡️ Moderator | 🟢 Green | Manage Messages, Kick/Ban | Điều hành viên |
| 🔧 Staff | 🔵 Blue | Manage Messages | Nhân viên hỗ trợ |
| 💎 Server Booster | 🟣 Purple | Special perks | Người boost server |
| ✅ Verified | 🟢 Green | Basic access | Thành viên đã verify |
| 👤 Member | ⚪ Gray | Basic access | Thành viên cơ bản |
| 🚫 Muted | ⚫ Dark Gray | No send messages | Bị mute |

### 📁 **Channel Structure**

```
🏠 SERVER NAME
├── 📖 THÔNG TIN CHUNG
│   ├── 🚪welcome
│   ├── 📋rules-and-info  
│   ├── 📢announcements
│   ├── 🎉events
│   └── ✅verification (nếu bật)
├── 💬 CHAT CHÍNH
│   ├── 💭general-chat
│   ├── 🎮gaming-talk (gaming template)
│   ├── 🖼️media-share
│   └── 🤖bot-commands
├── 🔊 VOICE CHANNELS
│   ├── 🎵Music Room
│   ├── 🎮Gaming Voice 1
│   ├── 🎮Gaming Voice 2
│   ├── 💬General Voice
│   └── 🔒Private Room
├── 🤖 BOT CHANNELS (nếu bật)
│   ├── 🤖mee6-commands
│   ├── 🤖carl-bot-commands
│   └── 🤖[custom-bot]-commands
├── 🎁 GIVEAWAY & EVENTS (nếu bật)
│   ├── 🎁giveaways
│   └── 🎊event-chat
├── 🛡️ STAFF AREA (Private - nếu bật)
│   ├── 👑owner-only
│   ├── ⚡admin-chat
│   ├── 🛡️mod-chat
│   ├── 🔧staff-general
│   └── 📊reports-logs
└── 🔞 NSFW (18+) (nếu bật)
    ├── 🔞nsfw-general
    └── 🔞nsfw-media
```

## 🛡️ Bảo mật

### ⚠️ **Quan trọng về User Token**

**NGUY HIỂM:**
- User Token có thể truy cập toàn bộ Discord account của bạn
- Không bao giờ chia sẻ token với người khác
- Sử dụng User Token có thể vi phạm Discord ToS

**AN TOÀN:**
- Chỉ sử dụng trên máy tính cá nhân
- Chỉ setup server của riêng bạn
- Đổi password Discord sau khi sử dụng (token sẽ invalid)
- Không lưu token ở nơi công cộng

### 🔒 **Best Practices**
```javascript
// Token sẽ được lưu tạm trong memory, không lưu persistent
// Tool không gửi token đến server nào khác
// Tất cả requests đều trực tiếp đến Discord API
```

## 🎛️ **Cấu hình nâng cao**

### 🔧 **Custom Bot Setup**
```javascript
// Thêm bots phổ biến:
const popularBots = [
    'MEE6',           // Moderation & Leveling
    'Carl-bot',       // Multi-purpose
    'Dyno',          // Moderation  
    'Mudae',         // Waifu game
    'Groovy',        // Music (deprecated)
    'Dank Memer',    // Memes & Economy
    'Ticket Tool',   // Support tickets
    'YAGPDB',        // Advanced automation
    'Pokecord',      // Pokemon game
    'Tatsu'          // Leveling & Social
];
```

### 🎨 **Template Customization**
```javascript
// Có thể tùy chỉnh templates:
const customTemplate = {
    name: "Custom Server",
    categories: [
        {
            name: "📋 CUSTOM CATEGORY",
            channels: [
                { name: "custom-channel", type: "text", topic: "Custom description" }
            ]
        }
    ]
};
```

## 📊 **API Rate Limits**

Tool tự động xử lý Discord rate limits:

| Action | Rate Limit | Tool Handling |
|--------|------------|---------------|
| Create Channel | 50/day | Queue system với delays |
| Create Role | 250/day | Batch processing |
| Edit Permissions | 10/10s | Rate limiter built-in |
| Send Messages | 5/5s | Auto retry với backoff |

## ❓ FAQ

### **Q: Tool có an toàn không?**
A: Tool chạy hoàn toàn client-side, không gửi dữ liệu đến server nào. Tuy nhiên việc sử dụng User Token có rủi ro vi phạm Discord ToS.

### **Q: Tại sao không dùng Bot Token?**
A: Bot Token không thể tạo channels/roles. Chỉ User Token mới có permissions đầy đủ để setup server.

### **Q: Tool có hoạt động với Vencord/BetterDiscord không?**
A: Có! Tool sử dụng Discord API nên hoạt động với mọi Discord client.

### **Q: Làm sao để undo nếu setup sai?**
A: Có thể dùng tính năng backup hoặc xóa channels/roles thủ công. Tool không có tính năng undo tự động.

### **Q: Tool có support server boost features không?**
A: Tool tạo cấu trúc cơ bản. Server boost features (banner, emoji slots, etc.) cần cấu hình thủ công.

## 🚨 **Troubleshooting**

### **Lỗi thường gặp:**

**❌ "Token không hợp lệ"**
```
Giải pháp:
1. Kiểm tra token có đúng format không
2. Đảm bảo đã copy đầy đủ (bỏ dấu ngoặc kép)
3. Thử refresh Discord web và lấy token mới
```

**❌ "Không có quyền"**
```
Giải pháp:
1. Kiểm tra có role Administrator không
2. Kiểm tra có phải Owner server không
3. Thử invite bot với quyền Administrator
```

**❌ "Rate limited"**
```
Giải pháp:
1. Tool sẽ tự động retry
2. Đợi 1-2 phút rồi thử lại
3. Không spam click setup button
```

**❌ "CORS Error"**
```
Giải pháp:
1. Dùng CORS extension cho browser
2. Hoặc chạy tool trên local server
3. Không mở từ file:// protocol
```

## 📱 **Compatibility**

### ✅ **Supported Discord Clients:**
- Discord Web (discord.com)
- Discord Desktop App
- Discord PTB/Canary
- Vencord
- BetterDiscord  
- AliCord
- Any Discord client with API access

### ✅ **Supported Browsers:**
- Chrome/Chromium 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## 🔄 **Updates & Roadmap**

### **v1.0.0 (Current)**
- ✅ Basic auto setup
- ✅ Templates system
- ✅ Bot integration
- ✅ Staff areas

### **v1.1.0 (Planned)**
- 🔄 Undo/Restore functionality
- 🔄 Advanced permissions editor
- 🔄 Bulk operations
- 🔄 Template sharing

### **v1.2.0 (Future)**
- 🔄 Bot invitation automation
- 🔄 Welcome message customization
- 🔄 Auto-moderation setup
- 🔄 Analytics dashboard

## 🤝 **Contributing**

### **Góp ý tính năng:**
1. Mở issue với tag `feature-request`
2. Mô tả chi tiết tính năng mong muốn
3. Giải thích use case và lợi ích

### **Report bugs:**
1. Mô tả chi tiết lỗi
2. Include browser console logs
3. Steps to reproduce
4. Expected vs actual behavior

### **Code contribution:**
```bash
# Fork repo
git clone your-fork
cd discord-auto-setup

# Tạo branch mới
git checkout -b feature-name

# Code và test
# Commit và push
git push origin feature-name

# Tạo Pull Request
```

## 📄 **License**

```
MIT License

Bạn có thể:
✅ Sử dụng cho mục đích cá nhân
✅ Modify và distribute
✅ Sử dụng thương mại

Điều kiện:
⚠️ Keep license notice
⚠️ Không warranty
⚠️ Tự chịu trách nhiệm khi sử dụng
```

## ⚠️ **Disclaimer**

```
🚨 QUAN TRỌNG:

1. Tool này KHÔNG PHẢI là official Discord tool
2. Sử dụng User Token có thể vi phạm Discord Terms of Service
3. Discord có thể suspend account nếu phát hiện automation
4. Chỉ sử dụng trên server riêng của bạn
5. Tool được tạo cho mục đích educational và personal use
6. Tác giả không chịu trách nhiệm về việc account bị ban
7. Sử dụng với trách nhiệm của riêng bạn
```

## 🆘 **Support**

### **Cần trợ giúp?**
- 📧 **Email:** your-email@example.com
- 💬 **Discord:** YourDiscord#1234
- 🐛 **Issues:** [GitHub Issues](https://github.com/your-repo/issues)
- 📖 **Wiki:** [Documentation](https://github.com/your-repo/wiki)

### **Community:**
- 🌐 **Discord Server:** [Join Community](https://discord.gg/your-invite)
- 💡 **Feature Requests:** [Request Features](https://github.com/your-repo/discussions)
- 🎥 **Video Tutorials:** [YouTube Channel](https://youtube.com/your-channel)

---

## 🎉 **Credits**

**Developed by:** Your Name  
**Inspired by:** Discord community needs  
**Special thanks:** Discord.js team, Discord API documentation

### **Used Technologies:**
- **Discord API v10** - Server automation
- **HTML5/CSS3/JS** - Frontend interface  
- **Fetch API** - HTTP requests
- **Local Storage** - Settings persistence (when available)

---

<div align="center">

**⭐ Nếu tool hữu ích, đừng quên star repo nhé! ⭐**

[🚀 Download Tool](https://your-link) | [📖 Documentation](https://github.com/your-repo/wiki) | [💬 Community](https://discord.gg/your-invite)

Made with ❤️ for Discord communities

</div>