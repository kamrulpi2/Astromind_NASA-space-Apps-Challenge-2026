# 🚀 Aqua Explorer: NASA's Hardware Across the Solar System

> An interactive educational game that lets school-age students explore the rovers, landers, instruments, and probes NASA has left across the Moon, Mars, and deep space.

**Built for the NASA Space Apps Challenge 2026**

[![Prototype](https://img.shields.io/badge/Prototype-Figma-F24E1E?logo=figma&logoColor=white)](https://www.figma.com/proto/OkwNxRuUFlf88F82MKg0HP/Nasa-space-app-challenge-2026?node-id=48-3&t=hzxmppfxNdOJ6Eyk-0&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=3%3A6&show-proto-sidebar=1)
[![Demo Video](https://img.shields.io/badge/Demo-YouTube-FF0000?logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=c4obotsspJE)
[![Data](https://img.shields.io/badge/Data-NASA%20Science-0B3D91)](https://science.nasa.gov/)
[![Status](https://img.shields.io/badge/Status-Prototype-orange)]()

---

## 📖 Table of Contents

1. [Overview](#-overview)
2. [The Challenge](#-the-challenge)
3. [Features](#-features)
4. [Featured Missions](#-featured-missions)
5. [How It Works](#-how-it-works)
6. [How We Developed This Project](#-how-we-developed-this-project)
7. [Tech Stack](#-tech-stack)
8. [Use of AI](#-use-of-artificial-intelligence)
9. [Data Sources](#-data-sources)
10. [Project Structure](#-project-structure)
11. [Getting Started](#-getting-started)
12. [Benefits](#-benefits)
13. [Roadmap](#-roadmap)
14. [Team](#-team)
15. [Disclaimer](#-disclaimer)
16. [Acknowledgments](#-acknowledgments)

---

## 🌍 Overview

Humans have sent rovers, landers, instruments, and probes to the Moon, Mars, and far beyond. Many are still working, and many have gone silent, but all of them taught us something about our solar system.

This project turns that story into a game. Instead of reading dense mission pages, students **explore missions, complete interactive challenges, and answer quizzes**. Each mission explains:

- 🛠️ **What the hardware is** and why it was built
- 🔬 **What scientific tasks it performed**
- 💡 **What discoveries it helped make**
- 📡 **What its status is today**

Storytelling, visuals, real science, and gameplay come together to make space exploration easier to understand and more fun.

## 🎯 The Challenge

NASA's hardware is spread across the solar system, but most students never learn where it is, what it did, or what it found. Our challenge was to **present this information in a way that is simple, visual, and engaging for school-age learners**, without losing scientific accuracy.

**How we addressed it:** we focused on rovers, landers, instruments, and probes located on the Moon, Mars, and in deep space. We converted complex mission data into easy-to-understand visuals, missions, and gameplay, so students learn by playing rather than memorizing.

## ✨ Features

| Feature | Description |
|---|---|
| 🎮 **Educational Game-Based Learning** | Learn by completing missions, not by reading walls of text |
| 🛰️ **NASA Hardware & Mission Exploration** | Browse rovers, landers, instruments, and probes by destination |
| 🧪 **Interactive Simulations** | Hands-on activities that show how the hardware works |
| 📊 **Real NASA Data Integration** | Mission facts based on publicly available NASA information |
| 📚 **Engaging Mission Narratives** | Each mission is told as a short story |
| ❓ **Interactive Quizzes & Challenges** | Test knowledge and earn progress |
| 📡 **Mission Status & Discoveries** | See whether each mission is active or complete, and what it found |
| 🧒 **User-Friendly Interface** | Designed for school-age students |

## 🛰️ Featured Missions

Missions are grouped by destination:

| 🌙 Moon | 🔴 Mars | 🌌 Deep Space |
|---|---|---|
| Landers & lunar instruments | Rovers & landers | Probes & orbiters (e.g., Cassini-Huygens) |

### Spotlight: Cassini-Huygens (Saturn)

> Data from [NASA Science: Cassini-Huygens](https://science.nasa.gov/mission/cassini/)

| | |
|---|---|
| **Type** | Orbiter and probe |
| **Launch** | October 15, 1997 |
| **Target** | The Saturn system |
| **Status** | ✅ Mission complete. Ended with the *Grand Finale* on September 15, 2017 |

**Purpose:** Cassini was a robotic spacecraft sent to study Saturn, its rings, and its family of icy moons in unprecedented detail.

**What it did:** It became the first spacecraft to orbit Saturn and began its in-depth study of the system in 2004, spending about 13 years there.

**Key discoveries:**
- Titan has methane rivers that flow into a methane sea.
- Enceladus has jets of ice and gas blasting from a liquid water ocean that may hold ingredients for life.
- Its "Backlit Saturn" image, taken on July 19, 2013, captured Saturn, its rings, seven moons, and Earth in the distance (*The Day the Earth Smiled*).

**Legacy:** Cassini's findings sparked a pivot toward exploring "ocean worlds." Its orbital tour design influenced NASA's Europa Clipper mission.

**Why it ended the way it did:** Nearly out of propellant, Cassini was deliberately sent into Saturn so it could not contaminate the moons, especially Enceladus and Titan, that scientists want to explore in the future.

> 🔧 *Add the remaining missions (Moon, Mars, other deep-space probes) here as your content is finalized.*

## 🎲 How It Works

```
Choose a destination  →  Pick a mission  →  Read the story
        ↓
Complete an interactive challenge  →  Take the quiz  →  Earn progress
        ↓
Unlock the next mission
```

1. **Explore:** the player picks a destination (Moon, Mars, or deep space).
2. **Learn:** each mission card shows the hardware, its purpose, discoveries, and current status.
3. **Play:** short challenges reinforce how the hardware works.
4. **Quiz:** questions check understanding and give instant feedback.

### Example mission data format

```json
{
  "id": "cassini-huygens",
  "name": "Cassini-Huygens",
  "destination": "Deep Space",
  "type": ["Orbiter", "Probe"],
  "launch": "1997-10-15",
  "target": "The Saturn System",
  "status": "Mission complete (Grand Finale: 2017-09-15)",
  "purpose": "Study Saturn, its rings, and its icy moons in detail.",
  "discoveries": [
    "Methane rivers and a methane sea on Titan",
    "Jets of ice and gas from a liquid water ocean on Enceladus"
  ],
  "quiz": [
    {
      "question": "Which moon of Saturn has jets blasting ice and gas into space?",
      "options": ["Titan", "Enceladus", "Europa", "Phobos"],
      "answer": "Enceladus"
    }
  ],
  "source": "https://science.nasa.gov/mission/cassini/"
}
```

## 🧭 How We Developed This Project

1. **Research:** studied NASA's missions and the hardware left across the solar system (rovers, landers, instruments, probes).
2. **Organize:** structured each mission's purpose, scientific contribution, and current status into a simple storyline.
3. **Design:** created an interactive game combining space visuals, storytelling, missions, and educational challenges.
4. **Integrate:** connected the collected NASA data with the game environment.
5. **Test:** checked that students can easily explore missions while learning the science and technology behind them.

## 🧰 Tech Stack

| Area | Tool |
|---|---|
| Prototyping & UI Design | **Figma** |
| Video Editing & Design | **Filmora** |
| Programming Language | `TODO: add language(s)` |
| Framework | `TODO: add framework(s)` |
| Mission Visuals & Promo Video | **Google Flow** |
| Game Design & Scripting Support | **ChatGPT** |

## 🤖 Use of Artificial Intelligence

We used AI tools to support design and content production. All mission facts were checked against NASA sources.

- **ChatGPT:** level design, game architecture, and video scripts.
- **Google Flow:** cinematic space scenes, mission visuals, and promotional video sequences.

## 📚 Data Sources

**NASA data**
- [NASA Science: Cassini-Huygens mission page](https://science.nasa.gov/mission/cassini/)
- [NASA Science](https://science.nasa.gov/) (mission pages for other featured hardware)
- [NASA Eyes on the Solar System](https://eyes.nasa.gov/apps/solar-system/) (mission timelines)

**Video references**
- [Project demo video](https://www.youtube.com/watch?v=c4obotsspJE)
- [Supporting reference video](https://www.youtube.com/watch?v=uddm93E3stE)

**Space agency partner & other data**
- `TODO: list any additional partner agencies or datasets used`

## 🗂️ Project Structure

> Update this to match your actual repository.

```
.
├── README.md
├── docs/
│   ├── design/            # Figma exports, screenshots
│   └── video/             # Demo video assets / links
├── data/
│   └── missions.json      # Mission content (purpose, discoveries, status)
├── src/
│   ├── game/              # Game logic, challenges
│   ├── quiz/              # Quiz engine and questions
│   └── ui/                # Screens and components
├── assets/                # Images, icons, audio
└── LICENSE
```

## 🚀 Getting Started

### Try the prototype
👉 [Open the interactive Figma prototype](https://www.figma.com/proto/OkwNxRuUFlf88F82MKg0HP/Nasa-space-app-challenge-2026?node-id=48-3&t=hzxmppfxNdOJ6Eyk-0&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=3%3A6&show-proto-sidebar=1)

### Watch the demo
▶️ [Project demo on YouTube](https://www.youtube.com/watch?v=c4obotsspJE)

### Run locally
```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
# TODO: add install and run commands for your stack
```

## 🎁 Benefits

- **Makes space science engaging:** students learn through interactive gameplay.
- **Improves scientific knowledge:** simple information about NASA missions, hardware, and discoveries.
- **Encourages curiosity:** inspires students to explore more about space and science.
- **Interactive learning:** combines education, storytelling, visuals, and challenges.
- **Easy to understand:** complex ideas presented in a user-friendly way.
- **Promotes STEM interest:** encourages interest in science, technology, engineering, and mathematics.

## 🔭 Roadmap

- [ ] Add more Moon, Mars, and deep-space missions
- [ ] Add difficulty levels by age group
- [ ] Add multi-language support
- [ ] Add teacher dashboard and classroom mode
- [ ] Sync mission status automatically from NASA sources
- [ ] Accessibility improvements (screen reader support, colorblind-friendly palette)

## 👥 Team

| Name | Role |
|---|---|
| `TODO` | `TODO` |

## ⚠️ Disclaimer

This project is for **educational and awareness purposes**, using publicly available information about NASA's missions and space hardware. It is **not an official NASA product** and is not endorsed by NASA. It is designed to encourage curiosity rather than replace detailed scientific resources. Mission status and discoveries may change as NASA continues its exploration.

## 🙏 Acknowledgments

- **NASA** and the **NASA Space Apps Challenge** for open data and inspiration
- NASA/JPL-Caltech and the Space Science Institute for Cassini imagery and mission information
- Everyone who tested the prototype and gave feedback

---

⭐ **If you like this project, please give it a star!**
