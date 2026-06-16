DevOS — Futuristic Developer New Tab Page
A clean, futuristic, and responsive Chrome New Tab/Home page designed for software engineers and developers. Built entirely with raw, self-contained HTML5, CSS3, and modern vanilla ES6+ JavaScript, DevOS delivers a sleek, cyberpunk-inspired workspace aesthetic without the bloat of heavy external frameworks or CDNs.
<p align="center">
<img src="https://img.shields.io/badge/License-MIT-00E5FF?style=flat-square" alt="MIT License">
<img src="https://img.shields.io/badge/PRs-welcome-7C4DFF?style=flat-square" alt="PRs Welcome">
<img src="https://img.shields.io/badge/Author-Ashu%20Yadav-00FF95?style=flat-square" alt="Author Ashu Yadav">
</p>
🌌 Theme & Visual Design
Style: Dark-mode cyberpunk, dashboard-driven, glassmorphism UI.
Layout: Standardized 3-column responsive grid (Bookmarks | Central Search | Diagnostics & Tasks).
Color Palette:
Primary Accent: Cyan (#00E5FF)
Secondary Accent: Purple (#7C4DFF)
Success/Active state: Mint Green (#00FF95)
Background: Interactive, lightweight HTML5 2D Canvas that renders a moving network of proximity-connected particles over an elegant code-grid texture.
🛠️ Key Features
1. Left Column: Bookmark Registry
Collapsible Categories: Group links logically into expandable and collapsible folder nodes (e.g., Development, Learning, AI Resources).
Dynamic Node Deployment: Easily add, edit, or purge bookmark cards and custom categories on the fly using safe local storage controls.
Smart Favicons: Generates clean site icons automatically. Fallbacks to procedural initials if a favicon is unavailable.
2. Center Column: Google Core Search
Sleek Interface: Rounded glassmorphic Google search bar positioned centrally.
Shortcut Capture: Pressing / instantly captures cursor focus on the search box, mimicking popular IDE workflows.
Diagnostic Panel: Includes a rotating selection of notable computer science and programming quotes.
3. Right Column: Diagnostics & Daily Tasks
Simulated Clock: Features a monospace, high-readability digital clock with a glowing neon footprint.
Live Meteorological Data: Automatically queries client geolocation (with safe fallbacks) to request real-time temperature, humidity, and weather description telemetry utilizing the free Open-Meteo API.
Daily Directives (Task List):
Add targets via an inline console bar.
Check off tasks with a fading strikethrough animation.
Automatic IST Midnight Reset: To align with developer productivity cycles, all active directives clear automatically at 00:00 IST (Indian Standard Time / Asia/Kolkata timezone) daily.
🚀 How to Install and Use
Option 1: Run Locally
Clone this repository to your machine:
code
Bash
git clone https://github.com/Ashu8833/DevOS-NewTab.git
Simply double-click the index.html file to launch it in your preferred browser.
Option 2: Set as Chrome New Tab Page (Recommended)
Because modern Chrome browsers require an extension to replace the default New Tab page, you can easily load DevOS as a local extension:
Create a file named manifest.json in the same directory as index.html with the following content:
code
JSON
{
  "manifest_version": 3,
  "name": "DevOS Workspace New Tab",
  "version": "1.0.0",
  "description": "Futuristic new tab workspace designed for developers.",
  "chrome_url_overrides": {
    "newtab": "index.html"
  },
  "permissions": ["geolocation"]
}
Open Google Chrome and navigate to chrome://extensions/.
Enable Developer mode (toggle switch in the top-right corner).
Click Load unpacked in the top-left corner.
Select the directory containing your index.html and manifest.json files.
Open a new tab and authorize the extension replacement when prompted.
🧬 Technology Stack
Markup & Structure: HTML5 (Clean, semantic tags)
Styling: Pure CSS3 variables, Flexbox, CSS Grid, custom keyframes, and glassmorphism.
Behavior: Modern Vanilla JS (ES6+) for event handling, localStorage sync, network canvas physics, and asynchronous API calls.
APIs:
Weather Data: Open-Meteo API (No API key required)
Location Resolution: Nominatim OpenStreetMap (Reverse Geocoding)
🔒 Security and Privacy
Zero External Trackers: DevOS is entirely offline-first. Your bookmark links, categories, and daily tasks never leave your computer.
Local Storage: All application data is stored locally in your browser's partition via standard localStorage APIs.
📄 License & Copyright
Copyright © 2026 Ashu Yadav (Ashu8833).
This project is open-source and released under the terms of the MIT License. Feel free to use, customize, modify, and distribute this template for personal or educational use.
code
Text
The MIT License (MIT)

Copyright (c) 2026 Ashu Yadav (Ashu8833)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
