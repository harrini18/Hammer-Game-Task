# Motocross Bike Game - Development Guide


## 🎯 Project Overview

Create a 2D side-scrolling motocross bike game where players collect strawberries across sky-island levels and reach a sunflower to complete each stage. The game emphasizes realistic bike physics, precise controls, and challenging obstacle navigation.


## 🧩 Core Game Features

### 1. Bike Physics System
- **Realistic Gravity:** Bike responds naturally to gravity and momentum
- **Air Control:** Tilt controls for landing balance and rotation management
- **Collision Detection:** Accurate collision system for crashes and safe landings
- **Rotation Mechanics:** 360-degree rotation capability for stunts and recovery

### Coin Economy
- **Earning:** 10 coins per completed level
- **Persistence:** Coin balance saved locally using Unity PlayerPrefs
- **Display:** Current coin count visible in Main Menu 
  
## 🖥 User Interface Requirements

### Main Menu
- **Level Selection:** Choose from 3 available levels
- **Bike Selection:** Switch between unlocked bikes
- **Coin Display:** Show current coin balance
- **Clean Design:** Intuitive navigation and visual feedback

### In-Game UI
- **Coin Counter:** Real-time coin display
- **Restart Button:** Manual level restart option
- **Timer:** Optional level completion timer
- **Minimalist Design:** Non-intrusive UI elements

## 🏗 Technical Implementation

### Scene Management
- **Single Scene Approach:** All gameplay within one Unity scene
- **Dynamic Loading:** Levels loaded/switched dynamically
- **Modular Design:** Reusable prefabs for quick level creation

### Prefab System
Create prefabs for:
- **Bike Models:** Both unlockable bikes
- **Level Elements:** Ramps, platforms, obstacles
- **Collectibles:** Strawberries and sunflower
- **UI Components:** Buttons, counters, menus
- **Traps:** Rotating bars, spikes, falling platforms

### Code Architecture
- **Modular C# Scripts:**
  - `BikeController.cs` - Main bike physics and controls
  - `GameManager.cs` - Level management and game state
  - `CoinSystem.cs` - Economy and save/load functionality
  - `LevelManager.cs` - Level switching and progress tracking
  - `UIManager.cs` - User interface management
  - `CrashDetection.cs` - Collision and restart logic


## 🧪 Testing Guidelines

### Control Testing
1. **Acceleration:** Smooth forward movement with W key
2. **Braking:** Effective speed reduction and reverse with S key
3. **Air Control:** Responsive tilt mechanics with A/D keys
4. **Rotation:** Natural bike rotation during jumps

### Physics Testing
1. **Landing Safety:** Proper landings don't trigger crashes
2. **Crash Detection:** Upside-down/sideways landings cause restart
3. **Obstacle Collision:** Heavy impacts trigger appropriate responses
4. **Gravity Feel:** Realistic fall speed and arc trajectories

### System Testing
1. **Save/Load:** Coins and unlocks persist between sessions
2. **Level Progression:** All 3 levels accessible and completable
3. **UI Functionality:** All buttons and displays work correctly
4. **Performance:** Stable 60fps on target platforms

## 📦 Submission Requirements

### File Structure
===================
### Deliverables
1. **Unity Project Files:** Complete project folder (.zip)
2. **WebGL Build:** Hosted online link for browser play
3. **README.txt:** Controls explanation and testing guide
4. **Build Instructions:** Steps to compile and run

### Quality Assurance
- **Error-Free:** Project opens without console errors
- **Complete Features:** All specified mechanics implemented
- **Playable Build:** WebGL version runs smoothly in browsers
- **Documentation:** Clear instructions for testing all features
## 📞 Development Notes

**Reference Game:** Moto X3M (Poki) - Use as inspiration for physics feel and control responsiveness, but focus on core mechanics rather than replicating all features.

**Key Focus Areas:**
1. **Smooth Controls:** Prioritize responsive, intuitive bike handling
2. **Fair Physics:** Ensure crashes feel justified, not random
3. **Clear Progression:** Make strawberry collection and goals obvious
4. **Stable Performance:** Maintain consistent framerate across all levels

---
