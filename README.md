# Discord Username Checker 💎

**Thanks for buying!** A Discord username checker

## ✨ What's Inside

- **Multi-Proxy support** - Works with any proxy format, validates automatically  
- **Smart generation** - Creates usernames by length (3-6 chars)
- **Saves Results** - Saves your hits by date
- **Live progress** - Shows progress as it runs

## 🚀 Let's Get Started

1. Run `discord-username-checker.exe`
2. Add your proxies to `proxies.txt` (file gets created on first run)
3. Pick how you want to check
4. the rest is automated

---

## 📋 Setup

### Proxies (You Need These)

Add them to `proxies.txt` - one per line:

```ini
http://user:pass@proxy.com:8080
socks5://proxy2.com:1080
user:pass@proxy.com:8080
proxy.com:8080
```

💡 **Need proxies?** Get some from [proxies.rip](https://proxies.rip/) - they work well

### Usernames (Optional)

Add specific usernames to check to `usernames.txt`:

```ini
username_i_want
womppp
damnthatsucks
```

---

## 🎮 How It Works

**[1] Check from file** - Checks your username list  
**[2] Generate by length** - Creates random usernames and checks them  
**[3] Settings** - See current settings
**[4] Exit** - Close the program

## 📁 Your Results

Everything gets saved in `hits/`:

```ini
hits/10-24-2025/available.txt
```

What you'll see:

```ini
@username1              ✅ Available
@username2              ✅ Available  
```

## ⚙️ Settings

Edit `config.json` if you want to change anything:

```json
{
  "threads": 10,
  "max_generate": 15,
  "min_length": 3,
  "max_length": 6
}
```

---

## 💬 Need Help?

**Message me:** @uhhhwhatever

- Setup help
- Questions about settings
- If something isn't working
- Ideas for new features

## ⚠️ Just So You Know

- **Needs proxies** - Won't work without them
- **This only checks** - it does not auto-register them
