# GitHub Contribution Viewer & 3D Skyline

A web-based visualization tool that displays a user's GitHub contribution graph and transforms it into a **3D skyline city**.

This project recreates the familiar GitHub contribution heatmap and converts contribution activity into buildings in a **3D city visualization using Three.js**.

Each contribution becomes a building where:

* **Contribution count → Building height**
* **Contribution intensity → Building color**
* **Date → City grid position**

---

# Features

### GitHub-style Contribution Graph

* Dark theme identical to GitHub
* Monthly and weekly layout
* Contribution intensity levels
* Tooltip for contribution counts

### Year Filtering

* Automatically detects available years
* Dropdown to switch between contribution years
* Updates graph and skyline dynamically

### 3D Contribution Skyline

* Built using **Three.js**
* Buildings generated from contribution data
* Height proportional to commit activity
* Window textures and lighting effects

### Interactive Controls

* Rotate the city (Left Mouse)
* Pan camera (Right Mouse)
* Zoom (Mouse Scroll)
* Reset camera view button

### Visual Enhancements

* Neon month separators
* Platform with month and day labels
* Building spires for high activity days
* Animated camera rotation

---

# Demo

Enter a GitHub username and visualize their contributions as a city skyline.

Example usernames to test:

```
torvalds
octocat
gaearon
```

---

# Technologies Used

* HTML5
* CSS3
* JavaScript
* Three.js (3D rendering)
* GitHub Contributions API

Libraries used:

* Three.js r128
* OrbitControls
* Canvas textures for building lighting

---

# How It Works

1. Fetch contribution data from the API:

```
https://github-contributions-api.jogruber.de
```

2. Convert the contribution calendar into a grid.

3. For each day:

```
contribution count → building height
contribution level → building color
date → city position
```

4. Render the buildings in a 3D scene using Three.js.

---

# Project Structure

```
github-contribution-viewer/
│
├── index.html
├── README.md
```

The entire application runs from a single HTML file.

---

# Installation

Clone the repository:

```
git clone https://github.com/soorajstudio/github-contribution-viewer.git
```

Open the project folder:

```
cd github-contribution-viewer
```

Run the project:

```
Open index.html in a browser
```

No build tools or installation required.

---

# Controls

| Action             | Result                |
| ------------------ | --------------------- |
| Left Click + Drag  | Rotate skyline        |
| Right Click + Drag | Pan camera            |
| Mouse Scroll       | Zoom                  |
| Reset View         | Reset camera position |

---

# Future Improvements

Possible enhancements:

* Export skyline as **3D printable STL**
* Add **city animation timeline**
* GitHub profile integration
* Real-time GitHub API authentication
* VR / WebXR skyline navigation
* Contribution comparison between users

---

# Author

Created by **Sooraj Studio**

GitHub:
https://github.com/soorajstudio

---

# License

MIT License

You are free to use, modify, and distribute this project.
