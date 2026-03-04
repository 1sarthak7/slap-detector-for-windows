<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=40&duration=3000&pause=1000&color=4CAF50&center=true&vCenter=true&multiline=true&repeat=true&width=700&height=100&lines=%F0%9F%96%90+SLAP+DETECTOR+%F0%9F%96%90;Slap+your+desk.+Get+a+reaction." alt="Typing SVG" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Audio-Real--Time-4CAF50?style=for-the-badge&logo=soundcharts&logoColor=white" />
  <img src="https://img.shields.io/github/license/1sarthak7/slap-detector-for-windows?style=for-the-badge&color=yellow" />
</p>

<p align="center">
  <img src="https://img.shields.io/github/stars/1sarthak7/slap-detector-for-windows?style=social" />
  <img src="https://img.shields.io/github/forks/1sarthak7/slap-detector-for-windows?style=social" />
  <img src="https://img.shields.io/github/watchers/1sarthak7/slap-detector-for-windows?style=social" />
</p>

---

<div align="center">

### 🎯 A real-time slap detection app for **Windows** that listens through your microphone, detects sharp impact sounds, and plays hilarious audio reactions.

*Built for Windows PCs • Real-time detection • Fun party trick 🎉*

</div>

---

#  Features

<table>
<tr>
<td width="50%">

### 🎤 Real-Time Audio Detection

Continuously monitors your microphone and processes audio blocks in real time to detect **sudden slap sounds** with minimal latency.

</td>
<td width="50%">

###  Live Visual Meter

```
🎤 [████████░░░░░░░░░░░░░░░░░░░░░░] peak=0.203
💥 SLAP DETECTED! Playing: meme_01.wav
```

Real-time terminal visualization of microphone intensity.

</td>
</tr>

<tr>
<td width="50%">

###  Adaptive Noise Detection

Automatically adapts to background noise using an **ambient noise baseline** so it works in quiet rooms and noisy environments.

</td>

<td width="50%">

### Random Sound Reactions

Drop `.wav` or `.mp3` files into the `audio/` folder and the program will **play a random sound** whenever a slap is detected.

</td>
</tr>
</table>

---

#  Quick Start

## Requirements

* **Windows 10 / Windows 11**
* **Python 3.9+**
* **Microphone**

---

# Installation

```bash
git clone https://github.com/1sarthak7/slap-detector-for-windows.git
cd slap-detector-for-windows

pip install sounddevice numpy playsound
```

---

# Run

```bash
python slap.py
```

Once running:

```
🎤 Listening for slaps...
```

Now **slap your desk or table** near the microphone and enjoy the reaction.

---

# ⚙️ Configuration

Edit these parameters at the top of `slap.py`:

| Parameter     | Default | Description                                   |
| ------------- | ------- | --------------------------------------------- |
| `THRESHOLD`   | `0.35`  | Minimum amplitude required to trigger         |
| `SPIKE_RATIO` | `3.0`   | How much louder than ambient the slap must be |
| `COOLDOWN`    | `1.0`   | Minimum seconds between triggers              |
| `SAMPLE_RATE` | `44100` | Microphone sample rate                        |
| `BLOCK_SIZE`  | `1024`  | Samples per analysis block                    |

---

# 🔧 Tuning Tips

```
Too many triggers? → Increase THRESHOLD
Missing slaps?     → Lower THRESHOLD
Double triggers?   → Increase COOLDOWN
Noisy room?        → Increase SPIKE_RATIO
```

---

# 📂 Project Structure

```
slap-detector-for-windows/
│
├── slap.py
├── audio/
│   ├── meme/
│   ├── pain/
│   └── random/
│
├── README.md
└── requirements.txt
```

---

#  How It Works

```mermaid
graph LR
A[🎤 Microphone] --> B[Audio Stream]
B --> C[Peak Detection]
C --> D{Above Threshold?}
D -->|Yes| E[💥 Slap Detected]
D -->|No| F[Update Ambient Noise]
E --> G[🔊 Play Random Sound]
E --> H[Cooldown Timer]
H --> B
F --> B
```

### Steps

1. Capture microphone audio
2. Analyze peak amplitude of each block
3. Compare against ambient noise baseline
4. If spike detected → trigger reaction
5. Play random sound from `audio/`

---

##  Contributing

<p align="center">
  <a href="https://github.com/1sarthak7/slap-detection-mac/issues">
    <img src="https://img.shields.io/badge/Report%20Bug-FF6B6B?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="https://github.com/1sarthak7/slap-detection-mac/issues">
    <img src="https://img.shields.io/badge/Request%20Feature-4CAF50?style=for-the-badge&logo=github&logoColor=white" />
  </a>
</p>

---

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=18&duration=4000&pause=2000&color=FF6B6B&center=true&vCenter=true&repeat=true&width=500&lines=Made+with+%E2%9D%A4%EF%B8%8F+and+a+lot+of+slapping+%F0%9F%96%90;by+%401sarthak7" alt="Footer" />
</p>

<p align="center">
  <a href="https://github.com/1sarthak7">
    <img src="https://img.shields.io/badge/GitHub-1sarthak7-181717?style=for-the-badge&logo=github" />
  </a>
</p>

<p align="center">
  ⭐ Star this repo if you enjoyed slapping Your lappy !
</p>
 
