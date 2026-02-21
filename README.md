# Dream Villa VR Experience

A comprehensive A-Frame VR experience featuring a modern villa with multiple rooms, animated swimming pool, and interactive elements.

## 🚀 Quick Start

**Live Demo:** Open `index.html` in your browser or deploy to GitHub Pages.

**GitHub Pages:** This repository is configured for GitHub Pages deployment. The site will be available at:
`https://VargasofJVD.github.io/ps-csc-22-0091-/`

## Features

✅ **Three Complete Rooms:**
- Living Room: Sofa, coffee table, TV, lamp, bookshelf, decorative plants
- Bedroom: Bed with pillows, wardrobe, bedside table, mirror, window
- Kitchen: Counter, stove, refrigerator, sink, table, chairs, cabinets

✅ **Animated Swimming Pool:**
- Multi-layer water animation with JavaScript-driven wave physics
- Pool walls and ladder
- Realistic water ripples effect

✅ **Additional Elements:**
- Trees (4 different trees with bark and leaves textures)
- Garden plants (multiple decorative plants)
- Vehicle (Lexus car model)
- Victorian street lamps with lighting
- Pet (animated dog with walking motion)

✅ **Lighting & Atmosphere:**
- Multiple light sources (ambient, directional, point lights)
- Shadow casting and receiving
- Fog effect for depth
- Sky with light blue color

✅ **Animations:**
- Pool water waves (JavaScript-driven)
- Furniture subtle movements
- Pet walking animation
- Tree swaying
- Lamp glow effects
- TV screen animation
- Stove flame animation

## Controls

- **WASD** or **Arrow Keys**: Move around
- **Mouse Drag**: Look around
- **VR Button**: Enter VR mode (if VR headset available)
- **ESC**: Exit VR mode

## File Structure

```
.
├── index.html                    # Main A-Frame scene (entry point)
├── modern_villa_for_sale.glb    # Villa 3D model
├── 2025_lexus_lx700h.glb        # Car model
├── victorian_street_lamp.glb    # Street lamp model
├── ground-grassColor.jpeg       # Grass texture
├── leaves-texture.webp          # Leaves texture
├── tree-bark-texture.jpg         # Tree bark texture
├── new-sky.jfif                  # Sky texture
├── DESIGN_DOCUMENT.md           # Design documentation
├── Design Document.pdf           # PDF version
└── README.md                     # This file
```

## Technical Implementation

### A-Frame Components Used:
- `gltf-model` - For 3D models (villa, car, lamps)
- `animation` - For various animations
- `movement-controls` - For camera movement
- `look-controls` - For head tracking
- `wasd-controls` - For keyboard navigation
- `shadow` - For realistic shadows
- `light` - Multiple light types

### Custom JavaScript:
- **Pool Water Animation**: JavaScript-driven wave system using `requestAnimationFrame`
  - Multiple wave layers with different frequencies and phases
  - Smooth, performant animation loop

## Browser Compatibility

- Chrome/Edge (recommended)
- Firefox
- Safari
- VR headsets: Oculus Quest, HTC Vive, etc.

## Performance Notes

- Optimized for 60 FPS on modern hardware
- Uses efficient primitive shapes where possible
- Shadow maps optimized for performance
- Fog culling for distant objects
- JavaScript-based pool animation for smooth performance

## Deployment

### GitHub Pages
1. Push code to GitHub repository
2. Go to Settings → Pages
3. Select branch: `main`
4. Select folder: `/ (root)`
5. Your site will be live at: `https://[username].github.io/[repo-name]/`

### Local Development
Simply open `index.html` in a modern web browser.

## Model Tuning

If models appear too large/small or in wrong positions, edit `index.html`:
- **Car**: Adjust `scale` and `position` on `#car` entity
- **Lamps**: Adjust `scale` and `position` on `#lamp-1`, `#lamp-2`, `#lamp-3`
- **Camera**: Initial position is `0 12 30` - adjust for different views

## Credits

- A-Frame Framework: https://aframe.io
- Physics System: aframe-physics-system
- Animation Component: aframe-animation-component
