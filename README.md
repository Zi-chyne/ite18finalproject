# Gado Racing Game

A browser-based racing game where you compete to achieve the fastest lap times. Race through the track, beat your best times, and see your scores on the leaderboard.

## Project Story & Concept

### The Story Behind Gado

**Gado** is a retro-inspired arcade racing game that brings the nostalgic thrill of classic racing games to the modern web browser. The name "Gado" evokes a sense of speed and adventure, capturing the essence of high-octane racing action.

The game was conceived as a tribute to the golden age of arcade racing games, where simple controls met challenging gameplay, and every lap was an opportunity to beat your personal best. In a world where racing games have become increasingly complex, Gado strips away the complexity and focuses on what makes racing fun: pure speed, skillful maneuvering, and the pursuit of perfection.

### Game Concept

**Gado** is a time-attack racing game that combines the visual style of classic arcade racers with modern web technologies. Players take control of a racing car and navigate through a dynamically generated track filled with curves, hills, and obstacles.

#### Core Gameplay Mechanics

1. **Time Attack Racing**: The primary objective is to complete the track in the shortest time possible. Every millisecond counts as you race against the clock, with your lap time displayed in minutes, seconds, and milliseconds format.

2. **Dynamic Track Generation**: Each race features a procedurally generated track that combines various elements:
   - **Curved Sections**: Navigate through winding roads that test your steering precision
   - **Elevation Changes**: Experience hills and valleys that add depth to the racing experience
   - **Straightaways**: Open sections where you can push your speed to the limit
   - **Environmental Elements**: Trees and scenery line the track, creating an immersive racing environment

3. **Traffic Management**: The track is populated with other vehicles that move at different speeds. Colliding with these cars will slow you down significantly, adding a strategic element to your racing line choices.

4. **Speed Control System**: 
   - **Acceleration**: Build up speed on straight sections
   - **Braking**: Slow down for tight corners or to avoid collisions
   - **Off-Road Penalty**: Straying too far from the center of the track reduces your maximum speed, encouraging players to stay on the racing line

5. **Leaderboard System**: After each race, your performance is recorded and displayed on a leaderboard. The game tracks your time, score (based on distance traveled), and lap time, allowing you to compete against yourself and strive for improvement.

#### Visual Design Philosophy

Gado embraces a retro aesthetic with modern polish:
- **Pixel-Perfect Art Style**: Inspired by classic arcade games, the visuals use a stylized approach that feels both nostalgic and fresh
- **Pseudo-3D Perspective**: The game uses a clever 2D rendering technique to create the illusion of 3D depth, reminiscent of classic racing games like Out Run
- **Optional 3D View**: For players who want a different perspective, the game includes an optional Three.js-powered 3D view that mirrors your car's movement
- **Dynamic Sky**: Animated cloud backgrounds add atmosphere and depth to the racing experience

#### Audio Experience

The game features a carefully crafted audio experience:
- **Theme Music**: An engaging soundtrack that sets the racing mood
- **Engine Sounds**: Dynamic engine audio that responds to your speed, making the car feel alive
- **Sound Effects**: Honk when you collide with other vehicles, beep countdown at the start, and other audio cues that enhance the gameplay

#### Technical Innovation

Gado demonstrates how modern web technologies can recreate classic gaming experiences:
- **Pure JavaScript**: Built without heavy game engines, showcasing the power of vanilla JavaScript
- **Canvas-Free Rendering**: Uses CSS and DOM manipulation for rendering, proving that great games don't always need canvas
- **Procedural Generation**: The track is generated algorithmically, ensuring each race feels unique
- **Performance Optimized**: Runs smoothly at 25 FPS, optimized for web browsers

#### The Challenge

Gado is more than just a racing game—it's a test of skill, precision, and persistence. The combination of:
- Tight time limits
- Challenging track layouts
- Traffic obstacles
- Speed management

Creates a gameplay loop that keeps players coming back to shave milliseconds off their best times. Whether you're a casual player looking for a quick race or a competitive player aiming for the top of the leaderboard, Gado offers an engaging experience that celebrates the pure joy of racing.

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- **Node.js** (version 12 or higher)
  - Download from [nodejs.org](https://nodejs.org/)
  - Verify installation by running: `node --version`
- **npm** (comes with Node.js)
  - Verify installation by running: `npm --version`
- A modern web browser (Chrome, Firefox, Edge, or Safari)

## Installation Steps

### Step 1: Clone or Download the Repository

If you have the repository URL:
```bash
git clone https://github.com/Zi-chyne/ite18finalproject.git
cd ite18finalproject
```

Or if you already have the files, navigate to the project directory:
```bash
cd ite18finalproject
```

### Step 2: Verify Project Structure

Ensure your project has the following structure:
```
ite18finalproject/
├── gado/
│   └── zion/
│       ├── index.html
│       ├── javascript/
│       │   ├── 1.js
│       │   └── main.js
│       ├── styles/
│       │   └── main.css
│       ├── images/
│       └── icon.png
├── package.json
└── server.js
```

### Step 3: Install Dependencies

This project uses only Node.js built-in modules, so no additional packages need to be installed. However, you can verify your setup:

```bash
npm install
```

This will ensure your `package.json` is properly configured (though no dependencies will be installed since none are required).

### Step 4: Start the Server

Run the development server:

```bash
npm start
```

Or directly with Node.js:

```bash
node server.js
```

You should see the following message:
```
Gado game running at http://localhost:8000/
```

### Step 5: Open in Browser

Open your web browser and navigate to:

```
http://localhost:8000/
```

The game should load and you'll see the Gado Racing game interface.

## How to Play

1. **Start the Game**: Press `C` to begin
2. **Controls**:
   - **Arrow Keys**: Steer left/right and accelerate/brake
   - **M**: Mute/unmute sound
3. **Goal**: Reach the finish line as fast as possible
4. **Leaderboard**: Your best lap times will appear on the leaderboard after each run

## Project Structure

```
ite18finalproject/
├── gado/
│   └── zion/              # Game assets and files
│       ├── index.html     # Main HTML file
│       ├── javascript/    # Game logic files
│       ├── styles/        # CSS styling
│       ├── images/        # Game images and assets
│       └── icon.png       # Game icon
├── package.json           # Node.js project configuration
├── server.js              # HTTP server for serving the game
└── README.md              # This file
```

## Technologies Used

- **Node.js**: Server runtime environment
- **HTML5/CSS3**: Frontend structure and styling
- **JavaScript**: Game logic and interactivity
- **Three.js**: 3D graphics library (loaded via CDN)

## Troubleshooting

### Port Already in Use

If port 8000 is already in use, you can set a different port:

```bash
PORT=3000 node server.js
```

Or on Windows PowerShell:
```powershell
$env:PORT=3000; node server.js
```

### Game Not Loading

1. Check that the server is running and you see the success message
2. Verify you're accessing `http://localhost:8000/` (not `http://localhost:8000/index.html`)
3. Check the browser console for any JavaScript errors
4. Ensure all files in the `gado/zion/` directory are present

### Node.js Not Found

If you get a "node is not recognized" error:
- Make sure Node.js is installed
- Restart your terminal/command prompt after installing Node.js
- Verify Node.js is in your system PATH

## Development

# Frontend
- **HTML5**: Structure of the game container and HUD
- **CSS3**: Styling for the UI, fonts, and animations
- **JavaScript**: Core game logic, rendering engine, and event handling
# Backend
- **Node.js**: A custom `server.js` script handles HTTP requests and serves static files
# Graphics Engine
- **Custom Pseudo-3D Engine**: Utilizes 2D DOM elements and projection math to create a 3D-like racing experience
# Pseudo-3D Projection
Uses a projection formula `project(camX, camY, camZ)` to map 3D world coordinates to the 2D screen, creating depth and perspective.
# Procedural Map Generation
The `genMap()` function constructs the track by pushing segments with varying curves and heights, creating a unique road layout for each race.
# Sprite Scaling
Sprites (trees, cars) are scaled based on their "Z" depth relative to the camera to simulate distance and create a sense of depth.
# Game Loop
Uses `requestAnimationFrame` for smooth rendering, calculating delta time to ensure consistent speed across different hardware configurations.


## Deployment

This project can be deployed to various platforms:

- **Vercel**: Already configured (see `.vercel` folder)
- **Heroku**: Add a `Procfile` with: `web: node server.js`
- **Any Node.js hosting**: Ensure the server runs on the platform's specified port

## Team Roles
Zion Andit – Main Developer
  Wrote the main code that makes the game run.
  Created the rules and logic for how the game plays.

Florence Libby Coles – Designer & Support Developer
  Designed the look, style, and visuals of the game.
  Helped program the user interface (menus and buttons).

## License

This project is private and proprietary.

## Support

For issues or questions, please check the project repository or contact the development team.
