# API Documentation

## Core Classes

### World

Main world class that manages the entire 3D scene and physics world.

```typescript
import { World } from 'sketchbook';

// Create world instance
const world = new World('scene.glb');
```

#### Constructor
- `constructor(scenePath: string)` - Load scene from GLB file

#### Main Methods
- `update(timeStep: number)` - Update world state
- `render()` - Render the scene
- `addCharacter(character: Character)` - Add character to world
- `addVehicle(vehicle: Vehicle)` - Add vehicle to world

### Character

Character control system with third-person controls support.

#### Key Features
- Capsule collision detection
- State machine system
- Animation blending
- AI behaviors

### Vehicle

Base class for vehicle system.

#### Subclasses
- `Car` - Automobile
- `Airplane` - Aircraft  
- `Helicopter` - Rotorcraft

## Physics System

Cannon.js physics engine integration:

- Rigid body physics
- Collision detection
- Constraint system
- Raycasting

## Rendering System

Three.js rendering pipeline:

- PBR materials
- Shadow mapping
- Post-processing effects
- FXAA anti-aliasing
