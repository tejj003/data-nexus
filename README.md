# Data Nexus - Interactive 3D Data Visualization

A stunning interactive 3D data visualization application built with Three.js that displays complex data patterns through beautiful animated visualizations.

![Data Nexus Preview](https://img.shields.io/badge/Status-Live-brightgreen)
![Three.js](https://img.shields.io/badge/Three.js-r128-blue)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## ✨ Features

### 🎨 Multiple Visualization Modes
- **Wave Field**: Dynamic wave patterns with mouse interaction
- **Particle Storm**: 5,000 animated particles with physics simulation
- **Neural Network**: Interactive node-based network with clickable elements
- **Data Galaxy**: Spiral galaxy formation with 8,000 stars

### 🎛️ Interactive Controls
- **Mouse Controls**: Click and drag to rotate the view
- **Zoom**: Mouse wheel to zoom in/out
- **Keyboard Shortcuts**: 
  - `Space`: Toggle auto-rotation
  - `R`: Reset camera view
  - `1-4`: Quick switch between visualization modes
- **Speed Control**: Adjustable animation speed slider
- **Theme System**: 4 color themes (Blue, Purple, Green, Orange)

### 🖥️ User Interface
- Clean, modern UI with glassmorphism design
- Real-time data metrics that change based on visualization mode
- Smooth animations and transitions
- Custom cursor with blend mode effects
- Loading screen with fade-in animations

## 🚀 Getting Started

### Prerequisites
- Modern web browser with WebGL support
- No additional dependencies required (Three.js loaded via CDN)

### Installation

1. **Clone or Download**
   ```bash
   git clone https://github.com/yourusername/data-nexus.git
   cd data-nexus
   ```

2. **Open in Browser**
   - Simply open `index.html` in your web browser
   - Or use a local server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   ```

3. **Access the Application**
   - Navigate to `http://localhost:8000` (if using local server)
   - Or open the HTML file directly

## 🎮 Usage Guide

### Navigation
- **Rotate View**: Click and drag anywhere on the visualization
- **Zoom**: Use mouse wheel to zoom in/out
- **Auto-Rotate**: Press `Space` to enable/disable automatic rotation
- **Reset**: Press `R` to return to default camera position

### Visualization Modes
1. **Wave Field** (`1` key)
   - Interactive wave simulation
   - Mouse position affects wave patterns
   - Perfect for demonstrating fluid dynamics

2. **Particle Storm** (`2` key)
   - 5,000 animated particles
   - Complex movement patterns
   - Ideal for representing data flow

3. **Neural Network** (`3` key)
   - 50 interconnected nodes
   - Click on nodes for pulse animation
   - Great for network topology visualization

4. **Data Galaxy** (`4` key)
   - Spiral galaxy with 8,000 stars
   - Color intensity based on distance
   - Excellent for hierarchical data

### Customization
- **Speed Control**: Use the slider in bottom-right to adjust animation speed
- **Color Themes**: Click color circles in the data panel to switch themes
- **Real-time Metrics**: Monitor different data points for each visualization mode

## 🛠️ Technical Details

### Technologies Used
- **Three.js**: 3D graphics and WebGL rendering
- **HTML5**: Semantic markup and structure
- **CSS3**: Modern styling with animations and glassmorphism
- **JavaScript ES6+**: Modern JavaScript features and classes

### Performance Features
- Efficient BufferGeometry for large particle systems
- Shader materials for complex visual effects
- Optimized rendering loop with requestAnimationFrame
- Responsive design with automatic viewport adjustment

### Browser Compatibility
- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+
- Requires WebGL support

## 📁 Project Structure

```
data-nexus/
├── index.html          # Main application file
├── README.md           # This file
└── assets/            # (Optional) Future assets directory
    ├── images/        # Screenshots, icons
    └── docs/          # Additional documentation
```

## 🎯 Data Metrics

Each visualization mode displays relevant metrics:

| Mode | Metric 1 | Metric 2 | Metric 3 | Metric 4 |
|------|----------|----------|----------|----------|
| Wave Field | Grid Points | Oscillations | Wave Flow | Field Load |
| Particle Storm | Particles | Interactions | Energy Flow | System Load |
| Neural Network | Active Nodes | Connections | Data Flow | Network Load |
| Data Galaxy | Stars | Clusters | Data Stream | Galaxy Load |

## 🎨 Customization

### Adding New Themes
1. Define colors in the `themes` object:
```javascript
this.themes = {
    // ...existing themes
    newTheme: { primary: 0xFFFFFF, secondary: 0x000000 }
};
```

2. Add theme button in HTML:
```html
<div class="theme-btn theme-new" data-theme="newTheme"></div>
```

3. Add corresponding CSS:
```css
.theme-new { background: #ffffff; }
```

### Creating New Visualizations
1. Add new mode to `switchMode()` method
2. Implement creation method (e.g., `createNewVisualization()`)
3. Add animation logic in `animate()` method
4. Update UI metrics in `updateUI()` method

## 🐛 Troubleshooting

### Common Issues
- **Blank Screen**: Check browser console for WebGL errors
- **Poor Performance**: Reduce particle count or disable antialiasing
- **Controls Not Working**: Ensure JavaScript is enabled

### Performance Tips
- Close other tabs for better performance
- Use Chrome for optimal WebGL performance
- Reduce animation speed if experiencing lag

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

### Development Guidelines
1. Follow existing code style and structure
2. Test across multiple browsers
3. Optimize for performance
4. Document new features

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Three.js](https://threejs.org/) - Amazing 3D library
- [WebGL](https://www.khronos.org/webgl/) - Web graphics standard
- Inspiration from data visualization pioneers

## 📞 Contact

- **Author**: Your Name
- **Email**: your.email@example.com
- **Project Link**: [https://github.com/yourusername/data-nexus](https://github.com/yourusername/data-nexus)

---

⭐ If you found this project helpful, please consider giving it a star!
