# CS2 Weapon Picker

An interactive Counter-Strike 2 weapon buy menu with random weapon spinner, drag-and-drop loadout customization, and faction-specific weapons.

## Features

### 🎲 Random Weapon Spinner
- **Pistol Round Spin** - Randomly selects from available pistols
- **Buy Round Spin** - Randomly selects from SMGs and rifles
- Animated highlighting with faction-colored glow
- Flashing winner animation

### 🎯 Faction-Specific Weapons
- **CT (Counter-Terrorist)** weapons: USP-S/P2000, M4A4, M4A1-S, FAMAS, AUG, etc.
- **T (Terrorist)** weapons: Glock-18, AK-47, Galil AR, SG 553, etc.
- Shared weapons: AWP, Desert Eagle, P90, etc.
- Molotov/Incendiary automatically switches based on faction

### 🔧 Loadout Customization
- **Drag-and-drop** weapons from bottom panel to equip slots
- **Click to unequip** weapons (returns them to available pool)
- **Starter pistol locked** - T-side Glock cannot be changed
- **CT starter pistol swap** - Switch between USP-S and P2000 in slot 1
- Separate loadouts for CT and T sides

### 💾 Persistent Storage
- Loadouts saved in browser localStorage
- Faction preference remembered
- All customizations persist across page reloads
- Independent CT and T loadout configurations

### 🎨 Authentic CS2 Styling
- Dark theme matching CS2 aesthetic
- Faction-colored UI elements (blue for CT, yellow for T)
- Responsive column layout

## How to Use

### Switching Factions
Click the faction toggle button in the top-right corner to switch between CT (blue) and T (yellow).

### Customizing Your Loadout
1. **Drag weapons** from the bottom "Dropped Weapons" panel into the slots above
2. **Starter pistols**: T-side Glock is locked, CT can swap between USP-S and P2000

### Using the Random Spinner
1. **Pistol Round** - Click to randomly highlight a pistol (includes starter pistol)
2. **Buy Round** - Click to randomly highlight an SMG or rifle
3. Watch the animated highlighting slow down and flash on the winner
4. Buttons are disabled during spin to prevent spam

### Resetting Everything
Open browser console (F12) and run:
```javascript
resetLoadout()
```
This clears all saved data and reloads with defaults.