# Development Guide

## Environment Setup

### System Requirements
- Node.js 16+ (LTS version)
- Modern browser with WebGL 2.0 support
- Local HTTP server

### Installation Steps

1. Clone repository
```bash
git clone https://github.com/swift502/Sketchbook.git
cd Sketchbook
```

2. Install dependencies
```bash
npm install
```

3. Start development server
```bash
npm run dev
```

4. Visit http://localhost:8080

## Project Structure

```
src/
├── ts/                 # TypeScript source code
│   ├── characters/     # Character system
│   ├── vehicles/       # Vehicle system
│   ├── physics/        # Physics engine
│   ├── world/          # World management
│   ├── core/           # Core functionality
│   ├── interfaces/     # Type definitions
│   └── enums/          # Enum types
├── css/                # Style files
├── img/                # Image assets
└── blend/              # Blender scene files
```

## Build System

### Development Mode
```bash
npm run dev
```
- Start webpack-dev-server
- Hot reload
- Source maps

### Production Build
```bash
npm run build
```
- Code minification
- Optimized output
- Type definitions generation

## Code Standards

### TypeScript Configuration
- Strict mode enabled
- ES2017 target
- Modular imports/exports

### Code Style
- TSLint rules
- 2-space indentation
- Semicolon endings
- camelCase naming

## Debugging Tips

### Browser Developer Tools
- Use Three.js Inspector extension
- Monitor performance panel
- Check WebGL state

### Physics Debugging
- Enable Cannon.js debug renderer
- Visualize collision bodies
- Monitor physics performance
