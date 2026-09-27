# Intelligent AR Indoor-Outdoor Navigation with an Embodied Robot Guide

> Final Year Project — Department of Information Sciences, University of Education, Lahore

## 📌 Abstract

University campuses are large, multi-building environments where new students, visitors, faculty and guests frequently struggle to reach a destination room, lab, or office, since GPS-based navigation tools work well outdoors but become unreliable indoors and do not model individual rooms, floors, or corridors. Existing indoor-navigation solutions such as Bluetooth beacons, QR codes, or Wi-Fi fingerprinting require costly infrastructure to be installed and maintained, making them impractical for most institutions. This project proposes an Intelligent Augmented Reality (AR) Indoor-Outdoor Navigation system that addresses this gap without any additional hardware. A person walks through a campus once using only a smartphone camera, allowing the system to "learn" the environment and build a reusable navigational map. Any subsequent user can then be guided using a world-locked AR path, accompanied by an animated 3D robot character that walks the route, waits for the user, and reacts to deviations. The system uses deterministic routing (A*) to ensure navigation remains reliable and never guides users through unlearned or invalid paths. It further extends across indoor-outdoor boundaries, transitioning seamlessly between AR guidance and standard outdoor GPS navigation. An AI-powered feature, using natural-language processing (NLP), allows users to ask questions such as room status or faculty availability directly from class-timetable data, offering alternate locations when a destination is closed. Together, these components form a practical, low-infrastructure, and engaging navigation solution suited to real university campuses.

## ✨ Key Features

- **Learn Mode** — record corridors, turns, stairs, lifts and destination points by walking through them once, with no fixed infrastructure required
- **World-locked AR Navigation** — turn-by-turn guidance rendered directly onto the real world through the phone camera
- **Embodied Robot Guide** — an animated 3D robot that walks the route, waits for the user, and reacts to deviations
- **Deterministic Routing** — A*-based path planning to ensure navigation is always reliable and never guesses an unverified route
- **Multi-floor Support** — handles stairs and lifts across multiple floors of a learned building
- **Indoor–Outdoor Continuity** — seamless hand-off between AR indoor guidance and standard outdoor GPS navigation
- **AI-Powered Room-Status & Faculty-Availability Lookup** — ask natural-language questions (e.g., *"Is Dr. Hanan free right now?"*) and get answers generated from timetable data via an NLP/LLM model, with alternate-location suggestions if a room is closed

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Engine / AR | Unity 6, AR Foundation, Google ARCore |
| Language | C# |
| Platform | Android SDK |
| 3D Modeling & Animation | Blender |
| Local Data Storage | JSON |
| AI / NLP | LLM API (e.g., Gemini / OpenAI / Claude API) |
| Data Source | Campus class timetable / schedule data (CSV/Excel) |
| Version Control | Git, GitHub |

## 📂 Project Structure

```
├── Assets/
│   ├── Scripts/          # Core navigation, routing, and AR logic
│   ├── Models/           # Robot guide 3D models and animations
│   ├── Scenes/           # Unity scenes
│   └── Data/             # Learned environment maps (JSON)
├── AI-Module/            # NLP/LLM integration for room-status & faculty lookup
├── Docs/                 # Proposal, diagrams, and documentation
└── README.md
```

## 🚀 Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/haseeb-muneer/<repo-name>.git
   ```
2. Open the project in **Unity 6** (with AR Foundation and Google ARCore packages installed).
3. Connect an ARCore-supported Android device for testing.
4. Build and deploy via **Android Studio** / Unity's Android build pipeline.

## 👥 Team

- Haseeb Muneer — [GitHub: haseeb-muneer](https://github.com/haseeb-muneer)
- Muhammad Naveed — [GitHub handle]
- Hassan Imran — [GitHub handle]

**Program:** BS Computer Science, University of Education, Lahore

## 📄 License

This project is developed as part of an academic Final Year Project. License to be added.
