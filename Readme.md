<h1 align="center">Villan Music Bot <\> </h1>

<p align="center">
  <img src="https://graph.org/file/9d75bfb77e17b80b3da5b.png" alt="Villan Music Logo" width="640" height="360">
</p>

<h2 align="center">Delivering Superior Music Experience To Telegram</h2>

---

### 🌟 Features

- 🎵 **Multiple Sources:** Play Music From Various Platforms.
- 📃 **Queue System:** Line Up Your Favorite Songs.
- 🔀 **Advanced Controls:** Shuffle, Repeat, And More.
- 🎛 **Customizable Settings:** From Equalizer To Normalization.
- 📢 **Crystal Clear Audio:** High-Quality Playback.
- 🎚 **Volume Mastery:** Adjust To Your Preferred Loudness.

---

<h3 align="center">
      ─「 <\> Deploy On Heroku <\> 」─
</h3>


### 🔧 Quick Setup

1. **Upgrade & Update:**

   ```bash
   sudo apt-get update && sudo apt-get upgrade -y
   ```

2. **Install Required Packages:**
   ```bash
   sudo apt-get install python3-pip ffmpeg -y
   ```
3. **Setting up PIP**
   ```bash
   sudo pip3 install -U pip
   ```
4. **Installing Node**
   ```bash
   curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash && source ~/.bashrc && nvm install v18
   ```
5. **Clone the Repository**
   ```bash
   git clone https://github.com/SahilKumarDev/villan-music-tg && cd VillanMusicBot
   ```
6. **Install Requirements**
   ```bash
   pip3 install -U -r requirements.txt
   ```
7. **Create .env with sample.env**
   ```bash
   cp sample.env .env
   ```
   - Edit .env with your vars
8. **Editing Vars:**
   ```bash
   nano .env
   ```
   - Press `I` Button On Keyboard To Start Editing.
   - Edit .env With Your Values.
   - Press `Ctrl + C` Once You Are Done With Editing Vars And Type `:wq` To Save .env Or `:qa` To Exit Editing.
9. **Installing tmux**
   ```bash
   sudo apt install tmux -y && tmux
   ```
10. **Run The Bot**
    ```bash
    bash start
    ```

---

### 🛠 Commands & Usage

The Villan Music Bot Offers A Range Of Commands To Enhance Your Music Listening Experience On Telegram:

| Command             | Description                             |
| ------------------- | --------------------------------------- |
| `/play <song name>` | Play The Requested Song.                |
| `/pause`            | Pause The Currently Playing Song.       |
| `/resume`           | Resume The Paused Song.                 |
| `/skip`             | Move To The Next Song In The Queue.     |
| `/stop`             | Stop The Bot And Clear The Queue.       |
| `/queue`            | Display The List Of Songs In The Queue. |

For A Full List Of Commands, Use `/help` in [Telegram]().

---

### 🔄 Updates & Support

Stay Updated With The Latest Features And Improvements To Villan Music Bot:


---

### 📜 License

This project Is Licensed Under The MIT License. For More Details, See The [LICENSE](LICENSE) File.

---


---
### Local Run By Docker

```bash
docker build -t villan-music:latest .
```

```bash
notepad .env
```


```bash 
API_ID=12345678
API_HASH=your_api_hash_here
BOT_TOKEN=your_bot_token_here
MONGO_DB_URI=mongodb://mongo:27017/villan
STRING_SESSION=your_string_session_here
OWNER_ID=123456789
LOG_GROUP_ID=-1001234567890
MUSIC_BOT_NAME=Villan Music
```

```bash
docker network create villan-network
```


```bash
docker run -d `
  --name villan-mongo `
  --restart unless-stopped `
  --network villan-network `
  -v mongo_data:/data/db `
  -p 27017:27017 `
  mongo:5.0
```


```bash
docker run -d `
  --name villan-music-bot `
  --restart unless-stopped `
  --env-file .env `
  --network villan-network `
  villan-music:latest
```


```bash
docker ps
```

```bash
docker logs -f villan-music-bot
```

---

### 🙏 Acknowledgements

Special Thanks To All The Contributors , Supporters , And Users Of The Villan Music Bot. Your Feedback And Support Keep Us Going !
