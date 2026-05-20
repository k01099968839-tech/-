# 테트리스 프로 - 모바일 최적화 버전

A mobile-optimized Tetris game built with vanilla HTML5, CSS3 (Tailwind), and JavaScript.

## 🎮 Features

### Core Gameplay
- **Classic Tetris Mechanics**: Standard 10×20 game board with 7 tetrominoes
- **7-Bag System**: Pseudo-random piece generation for balanced gameplay
- **Hold Piece**: Store and swap pieces for strategic gameplay
- **Ghost Block**: Preview where pieces will land
- **Wall Kick System**: Intelligent rotation with collision resolution
- **Scoring System**: Traditional line-clear scoring with level multipliers

### Mobile Optimizations
- **Touch Controls**: Responsive virtual d-pad and action buttons
- **Haptic Feedback**: Vibration on actions (drop, clear, game over)
- **Web Audio API**: Dynamic sound effects for all game actions
- **Responsive Canvas**: Auto-scaling game board to fit any screen size
- **Safe Area Support**: Respects device notches and safe zones
- **Gesture Prevention**: Disables unwanted pinch-zoom and scroll gestures

### UI/UX Features
- **Neon Design**: Purple-themed neon glow effects
- **Real-time Stats**: Live score, level, and line counter
- **Next/Hold Preview**: Mini-canvas displays for upcoming and held pieces
- **Pause System**: Full pause with game state preservation
- **Sound Toggle**: Mute sound effects without restarting
- **Game Over Screen**: Shows final score with restart option

## 🕹️ Controls

### Keyboard (Desktop)
| Key | Action |
|-----|--------|
| ← / → | Move left/right |
| ↑ | Rotate piece |
| ↓ | Soft drop |
| Space | Hard drop |
| C / Shift | Hold piece |
| P | Toggle pause |

### Mobile (Touch)
- **D-Pad**: Move and rotate pieces
- **HARD Button**: Fast drop with bonus points
- **HOLD Button**: Store current piece
- **Pause Button**: Pause/resume game
- **Sound Button**: Toggle audio

## 📊 Scoring

- **Soft Drop**: +1 point per cell
- **Hard Drop**: +2 points per cell
- **Line Clear**: 
  - 1 Line: 100 × Level
  - 2 Lines: 300 × Level
  - 3 Lines: 500 × Level
  - 4 Lines (Tetris): 800 × Level

## ⚡ Difficulty Progression

- **Level 1**: 1000ms drop interval
- Each new level: -90ms drop interval (minimum 100ms)
- **Level Up**: Every 10 lines cleared

## 🎨 Piece Colors

| Piece | Color | Type |
|-------|-------|------|
| I | Cyan (#06b6d4) | Straight |
| O | Yellow (#eab308) | Square |
| T | Purple (#a855f7) | T-shaped |
| S | Green (#22c55e) | S-shaped |
| Z | Red (#ef4444) | Z-shaped |
| J | Blue (#3b82f6) | J-shaped |
| L | Orange (#f97316) | L-shaped |

## 🔊 Sound Effects

- **Move**: Light beep (150→100 Hz)
- **Rotate**: Quick pitch up (200→350 Hz)
- **Drop**: Deep thud (100→40 Hz)
- **Line Clear**: Dual-tone success (C5 + E5)
- **Game Over**: Descending pitch (300→80 Hz)

## 🛠️ Technical Stack

- **HTML5 Canvas**: Game rendering engine
- **Web Audio API**: Dynamic sound synthesis
- **Vibration API**: Haptic feedback
- **Tailwind CSS**: UI styling and layout
- **Vanilla JavaScript**: Game engine and logic
- **RequestAnimationFrame**: 60fps game loop

## 📱 Browser Support

- Chrome/Edge 70+
- Firefox 63+
- Safari 12.1+
- Mobile browsers with HTML5 Canvas support

## 🚀 Getting Started

1. Clone or download the project
2. Open the HTML file in a web browser
3. Click "게임 시작" (Start Game) to begin
4. Use controls to play

### Desktop Testing
- Works great on any modern browser
- Use arrow keys for navigation
- Space for hard drop
- Press P to pause

### Mobile Testing
- Open on any smartphone or tablet
- Touch virtual buttons to play
- Haptic feedback on supported devices
- Optimized for landscape orientation

## ⚙️ Installation & Deployment

No build process required! Simply:
```bash
# Copy the HTML file to your web server
cp index.html /var/www/html/

# Or open directly in browser
open index.html
```

## 🎯 Game Rules

1. **Objective**: Clear lines by filling horizontal rows
2. **Game Over**: When a new piece can't spawn (collision at top)
3. **Hold**: Limited to one piece per turn
4. **Rotation**: Uses wall kick to prevent collision
5. **Ghost Block**: Shows landing position (cannot be disabled)

## 🐛 Known Limitations

- Audio context requires user interaction to activate (browser security)
- Some older devices may have limited haptic API support
- Landscape orientation recommended for optimal play

## 🔮 Future Enhancements

- [ ] Local storage high score persistence
- [ ] Multiplayer mode (socket.io)
- [ ] Difficulty presets (Easy/Normal/Hard)
- [ ] Statistics tracking (games played, avg score)
- [ ] Touch stick alternative controls
- [ ] Dark/Light theme toggle
- [ ] Accessibility improvements (screen reader support)

## 📄 License

Open source - feel free to modify and share!

## 👨‍💻 Author

Created as a mobile-first game experience showcase.

---

**Enjoy playing! 🎮**
