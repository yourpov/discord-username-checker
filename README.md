<div align="center">

# Discord Username Checker 💎

A simple Discord username checker with proxy support and username generation.

released after a year of gatekeeping

**Thanks for buying!**

</div>

# Showcase

https://github.com/user-attachments/assets/1c49921a-5ace-4da2-83e0-db068128f14c

## Features

* **Proxies**: supports multiple proxy formats
* **Generator**: generate usernames by length
* **Username list**: check usernames from a file
* **Progress**: see checks happen live
* **Hits**: saves available usernames by date

## Getting Started

1. Run `discord-username-checker.exe`
2. Add your proxies to `proxies.txt`
3. Pick how you want to check
4. the rest is automated

## Proxies

Add your proxies to `proxies.txt`, one per line:

```ini
http://user:pass@proxy.com:8080
socks5://proxy2.com:1080
user:pass@proxy.com:8080
proxy.com:8080
```

## Usernames

Add usernames you want to check to `usernames.txt`:

```ini
username_i_want
womppp
damnthatsucks
```

## Results

Hits are saved in the `hits/` folder:

```ini
hits/10-24-2025/available.txt
```

## Settings

Edit `config.json` to change the settings:

```json
```jsonc
{
  // How many checks run at once
  "threads": 50,

  // Delay between checks (ms)
  "delay": 500,

  // Request timeout (seconds)
  "timeout": 15,

  // Where your proxies are
  "proxy_file": "proxies.txt",

  // Check mode: "generate" or "file"
  "check_mode": "generate",

  // Min/max generated username length
  "min_length": 3,
  "max_length": 4,

  // Characters used for generated usernames
  "charset": "abcdefghijklmnopqrstuvwxyz1234567890",

  // How many usernames to generate
  "max_generate": 2000,

  // Username list when using "file" mode
  "username_file": "usernames.txt",

  // Folder to save results to
  "output_dir": "hits",

  // Save available usernames
  "save_valid": true,

  // Save unavailable usernames
  "save_invalid": false,

  // User-Agent sent with requests
  "user_agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",

  // Endpoint used for username checks
  "api_endpoint": "https://discord.com/api/v9/unique-username/username-attempt-unauthed",

  // Retries if a request fails
  "max_retries": 3,

  // Automatically slow down when needed
  "adaptive_delay": true,

  // Max adaptive delay (ms)
  "max_delay": 3000,

  // How much the delay increases each time
  "backoff_multiplier": 2.0
}
```

## Notes

* Proxies are required
* This only checks usernames
* It does not auto-register them

> yes, this is very old and the video looks like a typical youtube rat, it's not im just a bad editor lmao
> my username is no longer @uhhhwhatever get my latest contacts from https://yourpov.dev/
