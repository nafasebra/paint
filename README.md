# Canvas Paint Tool

A modern, web-based painting application built with HTML5 Canvas and JavaScript. This tool provides a comprehensive set of drawing features with an intuitive interface.

## 🎨 Features

### Drawing Tools
- **Pencil/Brush** - Freehand drawing with customizable brush sizes
- **Line Tool** - Draw straight lines between two points
- **Text Tool** - Add text annotations to your canvas
- **Rectangle** - Draw filled or outlined rectangles
- **Circle** - Draw filled or outlined circles
- **Rounded Rectangle** - Draw rectangles with rounded corners

### Canvas Controls
- **Zoom In/Out** - Scale your workspace for detailed work or overview
- **Pan** - Navigate around large canvases
- **Grid** - Optional grid overlay for precise alignment

### Export Options
- **PNG Export** - High-quality raster export
- **JPEG Export** - Compressed image export
- **Custom Resolution** - Choose export dimensions

### Additional Features
- **Undo/Redo** - Full history support
- **Color Picker** - Choose from palette or custom colors
- **Layer Support** - Work with multiple layers (planned)
- **Responsive Design** - Works on desktop and tablet devices

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/nafasebra/paint.git
cd paint
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:5173`

### Building for Production

```bash
npm run build
```

The built files will be in the `dist` directory.

## 🎯 Usage

### Basic Drawing
1. Select a drawing tool from the toolbar
2. Choose your desired color and brush size
3. Click and drag on the canvas to draw
4. Use the zoom controls to get closer for detailed work

### Shapes
1. Select Rectangle, Circle, or Rounded Rectangle tool
2. Click and drag to define the shape bounds
3. Release to create the shape
4. Hold Shift while dragging for perfect squares/circles

### Text
1. Select the Text tool
2. Click where you want to place text
3. Type your text in the input field
4. Press Enter to confirm or Escape to cancel

### Exporting
1. Click the Export button in the toolbar
2. Choose your preferred format (PNG/JPEG)
3. Set the desired resolution
4. Click Download to save your artwork

## 🛠️ Technical Stack

- **Frontend**: Vanilla JavaScript (ES6+)
- **Build Tool**: Vite
- **Canvas**: HTML5 Canvas API
- **Styling**: CSS3 with modern features
- **Module System**: ES Modules

## 📁 Project Structure

```
paint/
├── public/
│   └── vite.svg
├── src/
│   ├── components/
│   │   ├── Canvas.js
│   │   ├── Toolbar.js
│   │   └── ColorPicker.js
│   ├── tools/
│   │   ├── PencilTool.js
│   │   ├── LineTool.js
│   │   ├── TextTool.js
│   │   ├── RectangleTool.js
│   │   └── CircleTool.js
│   ├── utils/
│   │   ├── CanvasUtils.js
│   │   └── ExportUtils.js
│   ├── main.js
│   └── style.css
├── index.html
└── package.json
```

## 🎨 Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `P` | Pencil Tool |
| `L` | Line Tool |
| `T` | Text Tool |
| `R` | Rectangle Tool |
| `C` | Circle Tool |
| `+` / `Ctrl + +` | Zoom In |
| `-` / `Ctrl + -` | Zoom Out |
| `Ctrl + Z` | Undo |
| `Ctrl + Y` | Redo |
| `Ctrl + S` | Export PNG |
| `Space + Drag` | Pan Canvas |

## 🔧 Configuration

You can customize the paint tool by modifying the configuration in `src/config.js`:

```javascript
export const config = {
  canvas: {
    defaultWidth: 800,
    defaultHeight: 600,
    maxZoom: 500,
    minZoom: 10
  },
  tools: {
    defaultBrushSize: 5,
    defaultColor: '#000000'
  },
  export: {
    defaultFormat: 'png',
    quality: 0.9
  }
};
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and commit: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

## 📋 Roadmap

- [ ] Layer system implementation
- [ ] Brush texture support
- [ ] Vector shape tools
- [ ] Collaborative editing
- [ ] Mobile touch support optimization
- [ ] Plugin system
- [ ] Advanced filters and effects

## 🐛 Known Issues

- Large canvas sizes may impact performance on older devices
- Touch gestures need optimization for mobile devices
- Undo history is limited to prevent memory issues

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with [Vite](https://vitejs.dev/) for fast development
- Inspired by popular painting applications
- Canvas API documentation from [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)

## 📞 Support

If you encounter any issues or have questions:
- Create an issue on GitHub
- Check the [Wiki](../../wiki) for detailed documentation
- Join our [Discussions](../../discussions) for community support

---

Made with ❤️ by [nafasebra](https://github.com/nafasebra)
