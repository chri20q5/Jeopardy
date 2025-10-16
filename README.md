# 🎯 HTW Jeopardy

A modern, browser-based Jeopardy-style game with dual-screen support, perfect for classroom or party game nights!

![License](https://img.shields.io/badge/license-MIT-blue.svg)

## ✨ Features

- 🎮 **Fully Customizable Game Board** - Configure columns (1-12) and rows (1-10)
- 🏷️ **Category Titles** - Name your categories
- ❓ **Question & Answer Management** - Easy setup interface
- 👥 **Team Management** - Add unlimited teams with score tracking
- 📺 **Dual Screen Support** - Control panel + display window for secondary screen
- 💾 **Save/Load Game Setups** - Export/import via JSON files
- 🎊 **Visual Effects** - Confetti for correct answers, screen shake for wrong answers
- 🔊 **Sound Effects** - Audio feedback for scoring
- 🔄 **Game Reset** - Reset scores and questions without losing setup
- 💯 **Automatic Point Calculation** - Points increment by 100 per row (100, 200, 300...)
- ✅ **Question Tracking** - Used questions are grayed out
- 🎨 **Classic Jeopardy Design** - Modern take on the iconic blue aesthetic

## 🚀 Quick Start

### Installation

1. **Clone or download this repository**
   ```bash
   git clone <your-repo-url>
   cd Jeopardy
   ```

2. **Open `index.html` in your web browser**
   - Double-click the file, or
   - Right-click → Open with → Your preferred browser

That's it! No installation, no dependencies, no server required.

## 📖 How to Use

### Step 1: Setup Your Game

1. Open `index.html` in your browser
2. **Configure Grid**:
   - Set number of categories (columns)
   - Set number of questions per category (rows)
   - Click "Generate Board"
3. **Fill in Content**:
   - Enter category names
   - Add questions and answers for each cell
4. **Add Teams**:
   - Enter team names
   - Click "Add Team"
5. **Save Your Setup** (optional):
   - Click "💾 Save Setup" to export as JSON
   - Load it later with "📂 Load Setup"

### Step 2: Start the Game

1. Click **"▶️ START GAME"**
2. A new window opens automatically - this is your **display screen**
3. **Move the display window** to your secondary monitor/projector
4. **Keep the control panel** on your main screen

### Step 3: Play!

**On the Display Screen (players see this):**
- Click a cell to reveal the question
- Click the question to reveal the answer

**On the Control Panel (you see this):**
- View both question AND answer simultaneously
- Award points to teams using +/− buttons
- Points are based on the current question's value
- Teams can go negative

**Visual Feedback:**
- ✅ **Positive points**: Confetti animation + success sound
- ❌ **Negative points**: Screen shake + buzzer sound

### Step 4: Game Management

**During the game:**
- **Clear Current Question** - Remove current question display
- **🔄 Reset Game** - Reset all scores and questions (keeps your setup)
- **End Game** - Return to setup screen

**In setup screen:**
- **Reset All Scores** - Set all team scores back to 0

## 💾 Save & Load

### Saving
- Click "💾 Save Setup" to download a JSON file
- Contains: grid size, categories, questions, and answers
- **Does NOT save**: teams or game progress

### Loading
- Click "📂 Load Setup" and select a JSON file
- Your existing teams are preserved
- Perfect for switching between different game topics!

## 🎨 Customization

### Point Values
By default, points increment by 100 per row:
- Row 1: 100 points
- Row 2: 200 points
- Row 3: 300 points
- etc.

This automatically adjusts if you add more rows!

### Grid Sizes
- **Default**: 6 columns × 5 rows (classic Jeopardy)
- **Supported**: 1-12 columns, 1-10 rows
- Example: 8 columns × 6 rows = 48 questions

## 🖥️ Browser Compatibility

Works in all modern browsers:
- ✅ Chrome/Edge (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Opera

**Requirements:**
- JavaScript enabled
- Pop-up blocker disabled (for display window)
- Modern browser (2020+)

## 📱 Multi-Screen Setup

### Recommended Setup:
1. **Laptop + External Monitor**:
   - Control panel on laptop screen
   - Display window on external monitor

2. **Laptop + Projector**:
   - Control panel on laptop
   - Display window on projector
   - Set projector to "Extended Display" mode

3. **Desktop with Multiple Monitors**:
   - Drag display window to secondary monitor
   - F11 on display window for fullscreen

## 🎓 Use Cases

- 📚 **Classroom Review Games** - Make learning fun!
- 🎉 **Party Entertainment** - Test your friends' knowledge
- 🏢 **Corporate Training** - Gamify training sessions
- 👨‍👩‍👧‍👦 **Family Game Night** - Create custom trivia

## ⌨️ Keyboard Shortcuts

**Display Screen:**
- `ESC` - Close current question
- `Space/Enter` - Reveal answer

**Control Panel:**
- `ESC` - Clear current question (during game)

## 🔧 Technical Details

- **Frontend Only** - Pure HTML, CSS, and JavaScript
- **No Server Required** - Runs entirely in the browser
- **No Dependencies** - No frameworks, no build process
- **Data Storage**: 
  - LocalStorage for auto-save during session
  - JSON export/import for permanent storage
- **Communication**: BroadcastChannel API + Storage Events for window sync

## 📝 File Structure

```
Jeopardy/
├── index.html       # Control panel (main screen)
├── display.html     # Display screen (secondary monitor)
└── README.md        # This file
```

## 🤝 Contributing

Feel free to fork and customize for your needs! Some ideas:
- Add timer functionality
- Custom color themes
- Daily Double support
- Final Jeopardy round
- Different point systems

## 📄 License

MIT License - feel free to use, modify, and distribute!

## 🐛 Troubleshooting

### Display window doesn't open
- **Check pop-up blocker** - Allow pop-ups for the page
- **Try manually** - If auto-open fails, right-click `display.html` → Open in new window

### Windows don't sync
- **Refresh both windows** - The game state will reload from localStorage
- **Check browser console** - F12 → Console for any errors

### Confetti/effects not showing
- **Check browser compatibility** - Use a modern browser
- **Refresh the display window** - Sometimes needs a restart

### Sound not playing
- **Check volume** - System and browser volume
- **Browser autoplay policy** - Some browsers block audio until user interaction

## 💡 Tips & Tricks

1. **Prepare setups in advance** - Create and save multiple JSON files for different topics
2. **Test before presenting** - Run through at least one question to ensure sync works
3. **Fullscreen mode** - Press F11 on display window for immersive experience
4. **Keep teams simple** - 2-4 teams works best for gameplay
5. **Vary difficulty** - Put easier questions in top rows, harder in bottom rows

## 🎯 Made For

HTW (Hochschule für Technik und Wirtschaft) - but customizable for any use case!

---

**Enjoy your game! 🎊**

For questions or issues, please open an issue on GitHub.
