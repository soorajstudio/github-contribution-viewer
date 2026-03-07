# AIYOOO - Cyber-City GitHub Visualizer

A web-based visualization tool that displays a user's GitHub contribution graph and transforms it into a **3D cyberpunk skyline city**.

This project recreates the familiar GitHub contribution heatmap and converts contribution activity into buildings in a **3D city visualization using Three.js**, complete with CRT scanlines, neon glows, and an integrated audio engine.

Each contribution becomes a building where:

* **Contribution count → Building height**
* **Contribution intensity → Building color (Cyan, Magenta, Violet, Neon Green)**
* **Date → City grid position**

---

# 🚀 Live Demo

🌐 **Try the project here:**
https://gitcybercity.netlify.app/

Enter a GitHub username and visualize their contributions as a **3D cyberpunk skyline city**.

Example usernames to test:

```id="7s3rnx"
torvalds
octocat
gaearon
```

---

# ✨ Features

## Cyberpunk Contribution Dashboard

* Deep void dark theme with CRT scanlines and noise grain
* Monthly and weekly matrix layout
* Hover tooltips for contribution counts and dates
* Integrated audio engine with visualizer and volume control

## Year Filtering

* Automatically detects available years
* Dropdown to switch between contribution years
* Updates 2D graph and 3D skyline dynamically

## 3D Contribution Skyline

* Built using **Three.js**
* Buildings generated from contribution data
* Height proportional to commit activity
* Holographic spinning rings, neon laser beams, and glowing beacons

## Interactive Controls

* Rotate the city *(Left Mouse)*
* Pan camera *(Right Mouse)*
* Zoom *(Mouse Scroll)*
* Reset camera view button

## Visual Enhancements

* Custom shaders and glowing neon materials
* Velocity-based continuous camera rotation physics
* Animated audio visualizer synced to the music player
* Base platform with illuminated edges

---

# 🛠 Technologies Used

* **React 18**
* **TypeScript**
* **Vite**
* **CSS3** *(Custom CRT and Neon styles)*
* **Three.js** *(3D rendering)*
* **GitHub Contributions API**

Libraries used:

* Three.js
* React Hooks (`useState`, `useEffect`, `useRef`)

---

# ⚙️ How It Works

1. Fetch contribution data from the API:

```id="p98dcr"
https://github-contributions-api.jogruber.de
```

2. Convert the contribution calendar into a grid.

3. For each day:

```id="p1b6z3"
contribution count → building height
contribution level → neon building color & holographic effects
date → city position
```

4. Render the buildings in a **3D scene using Three.js**.

---

# 📂 Project Structure

```id="mjnbfa"
git-cyber-city/
│
├── public/
├── src/
│   ├── App.tsx          # Main React interface and Audio Engine
│   ├── CityRenderer.ts  # Three.js 3D generation logic
│   ├── index.css        # Cyberpunk styling and animations
│   └── types.ts         # TypeScript interfaces
│
├── index.html
├── package.json
├── vite.config.ts
└── README.md
```

---

# 💻 Installation

Clone the repository:

```id="hyglfd"
git clone https://github.com/soorajstudio/git-cyber-city.git
```

Open the project folder:

```id="9y85pl"
cd git-cyber-city
```

Install dependencies:

```id="fyig8t"
npm install
```

Run the project:

```id="2mnntg"
npm run dev
```

---

# 🎮 Controls

| Action             | Result                |
| ------------------ | --------------------- |
| Left Click + Drag  | Rotate skyline        |
| Right Click + Drag | Pan camera            |
| Mouse Scroll       | Zoom                  |
| Reset View         | Reset camera position |

---

# 🔮 Future Improvements

Possible enhancements:

* Export skyline as **3D printable STL**
* Add **city animation timeline**
* GitHub profile integration
* Real-time GitHub API authentication
* VR / WebXR skyline navigation
* Contribution comparison between users

---

# 👨‍💻 Author

Created by **Sooraj Studio**

GitHub:
https://github.com/soorajstudio

---

# 📜 License

MIT License

You are free to **use, modify, and distribute** this project.
