# Hacking Simulation - Matrix Style Terminal

A visually stunning, movie-style hacking simulation featuring Matrix-inspired falling code, dual split-screen terminals, realistic sound effects, and native window-styled popup alerts.

## 🎬 Features

### Visual Effects
- **Matrix Background**: Authentic falling code animation with green characters
- **Split Terminal Mode**: Dual side-by-side terminals running simultaneous hacking sequences
- **Native Window Popups**: macOS-style alert windows with realistic titlebar and control buttons
- **Smooth Animations**: Typewriter effect, progress bars, and smooth transitions
- **Terminal Aesthetics**: Professional monospace fonts (Fira Code, Share Tech Mono)

### Interactive Elements
- **Auto-scroll**: Terminals automatically scroll to show latest activity
- **Infinite Loop**: Simulation runs continuously, clearing and restarting
- **Progress Bars**: ASCII-style progress indicators `[████████░░] 80%`
- **File Downloads**: Simulated file transfer with individual progress tracking
- **Alert Popups**: Multiple cascading warning windows

### Audio Experience
- **Ambient Soundtrack**: Low-frequency background drone for atmosphere
- **Typing Sounds**: Randomized keyboard clicks for realism
- **Success Tones**: Melodic chords for successful operations
- **Warning Beeps**: Alert sounds for critical events
- **Progress Notifications**: Audio feedback when operations complete

### Responsive Design
- **Desktop**: Full split-screen experience with both terminals
- **Mobile**: Single terminal (Terminal A) optimized for smaller screens
- **Automatic Detection**: Switches layout based on screen width (768px breakpoint)

## 🚀 Quick Start

### Option 1: Direct Open
1. Download `index.html`
2. Double-click to open in your default browser
3. Simulation starts automatically after 1 second

### Option 2: Local Server (Recommended)
```bash
# Using Python 3
python3 -m http.server 8000

# Using Node.js
npx http-server

# Then open: http://localhost:8000
```

## 🎮 Usage

- **Start**: The simulation begins automatically when the page loads
- **Audio**: Click anywhere on the page to enable sound (browser autoplay policy)
- **Fullscreen**: Press `F11` or use browser's fullscreen option for immersive experience
- **Stop**: Close the browser tab or refresh the page

## 🛠️ Technical Details

### Technologies Used
- **HTML5**: Canvas API for Matrix effect
- **CSS3**: Animations, keyframes, responsive design
- **JavaScript**: Web Audio API for sound generation
- **Google Fonts**: Fira Code and Share Tech Mono

### Browser Compatibility
- ✅ Chrome/Edge (Latest)
- ✅ Firefox (Latest)
- ✅ Safari (Latest)
- ✅ Opera (Latest)

**Note**: Web Audio API requires user interaction on some browsers. Click the page to enable sound.

## 🎨 Customization

### Adjust Animation Speed
Find the `hackingSequenceLeft` and `hackingSequenceRight` arrays and modify `delay` values (in milliseconds):
```javascript
{ text: "Scanning network...", delay: 600, class: "command" }
//                                    ^^^
//                          Lower = Faster, Higher = Slower
```

### Change Colors
Modify CSS color variables:
```css
.line { color: #0f0; }        /* Terminal text - green */
.command { color: #0ff; }      /* Commands - cyan */
.warning { color: #ff0; }      /* Warnings - yellow */
.success { color: #0f0; }      /* Success - green */
```

### Disable Sound
Set `soundEnabled` to `false`:
```javascript
let soundEnabled = false;
```

### Modify Terminal Content
Edit the `hackingSequenceLeft` and `hackingSequenceRight` arrays to add/remove/modify terminal output.

## 📱 Responsive Breakpoints

- **Desktop** (> 768px): Split-screen with both terminals
- **Mobile** (≤ 768px): Single terminal, Terminal B hidden

## ⚠️ Disclaimer

This is a **simulation for educational and entertainment purposes only**. It does not perform any actual hacking, network scanning, or unauthorized access. All operations are purely visual effects.

**Do not use this to:**
- Intimidate or deceive others
- Pretend to perform illegal activities
- Violate any laws or regulations

## 📄 License

Free to use for personal and educational projects. Attribution appreciated but not required.

## 🤝 Contributing

Feel free to fork, modify, and enhance! Some ideas:
- Add more hacking sequences
- Create different terminal themes (Windows CMD, Linux, etc.)
- Add keyboard shortcuts
- Implement sound toggle button
- Add more popup variations

## 🎓 Educational Use

Perfect for:
- Learning web animations and Canvas API
- Understanding Web Audio API
- Practicing responsive design
- Creating movie/presentation props
- Demonstrating cybersecurity concepts visually

---

**Made with 💚 and JavaScript**

*For the best experience, use fullscreen mode and enable audio!*
