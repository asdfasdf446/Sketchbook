# Tutorial

## Quick Start

### Basic Scene Creation

```javascript
// 1. Import Sketchbook
import { World } from 'sketchbook';

// 2. Create world
const world = new World();

// 3. Load scene
world.loadScene('path/to/scene.glb');
```

### Adding Characters

```javascript
import { Character } from 'sketchbook';

// Create character
const character = new Character();
world.addCharacter(character);

// Set character position
character.setPosition(0, 0, 0);
```

## Blender Scene Creation

### Scene Setup
1. Create scene in Blender
2. Set physics properties (collision bodies)
3. Export as GLB format

### Naming Conventions
- Collision bodies: end with "_collision"
- Spawn points: end with "_spawn"
- Triggers: end with "_trigger"

### Material Setup
- Use PBR materials
- Ensure correct texture paths
- Optimize texture sizes

## Character Controls

### Keyboard Controls
- WASD: Movement
- Space: Jump
- Shift: Run
- Mouse: Camera control

### Custom Controls
```javascript
// Bind custom key
world.inputManager.bind('customAction', 'KeyE');

// Listen for key events
world.inputManager.on('customAction', () => {
    // Execute custom action
});
```

## Vehicle System

### Cars
```javascript
import { Car } from 'sketchbook';

const car = new Car();
world.addVehicle(car);

// Enter vehicle
character.enterVehicle(car);
```

### Airplanes
```javascript
import { Airplane } from 'sketchbook';

const plane = new Airplane();
world.addVehicle(plane);
```
