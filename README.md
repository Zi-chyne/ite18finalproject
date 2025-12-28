# Gado Racing Game

A browser-based racing game where you compete to achieve the fastest lap times. Race through the track, beat your best times, and see your scores on the leaderboard.

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
git clone <repository-url>
cd 21
```

Or if you already have the files, navigate to the project directory:
```bash
cd 21
```

### Step 2: Verify Project Structure

Ensure your project has the following structure:
```
21/
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
21/
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

## Deployment

This project can be deployed to various platforms:

- **Vercel**: Already configured (see `.vercel` folder)
- **Heroku**: Add a `Procfile` with: `web: node server.js`
- **Any Node.js hosting**: Ensure the server runs on the platform's specified port

## Uploading to GitHub

Follow these steps to upload your project to GitHub:

### Prerequisites for GitHub

- **Git** installed on your system
  - Download from [git-scm.com](https://git-scm.com/)
  - Verify installation: `git --version`
- A **GitHub account**
  - Sign up at [github.com](https://github.com/) if you don't have one

### Step 1: Initialize Git Repository

Open your terminal/command prompt in the project directory and run:

```bash
git init
```

### Step 2: Add All Files

Add all project files to Git:

```bash
git add .
```

### Step 3: Create Initial Commit

Commit your files:

```bash
git commit -m "Initial commit: Gado Racing Game"
```

### Step 4: Create GitHub Repository

1. Go to [github.com](https://github.com/) and sign in
2. Click the **"+"** icon in the top right corner
3. Select **"New repository"**
4. Enter a repository name (e.g., `gado-racing-game`)
5. Choose **Public** or **Private** (as per your preference)
6. **Do NOT** initialize with README, .gitignore, or license (we already have these)
7. Click **"Create repository"**

### Step 5: Connect Local Repository to GitHub

After creating the repository, GitHub will show you commands. Use these (replace `<your-username>` and `<repository-name>` with your actual values):

```bash
git remote add origin https://github.com/<your-username>/<repository-name>.git
git branch -M main
git push -u origin main
```

**Note**: If you're using GitHub with authentication, you may need to:
- Use a Personal Access Token instead of password
- Or set up SSH keys for authentication

### Step 6: Verify Upload

1. Refresh your GitHub repository page
2. You should see all your files including the README.md
3. The README will automatically display on the repository's main page

### Alternative: Using GitHub Desktop

If you prefer a graphical interface:

1. Download [GitHub Desktop](https://desktop.github.com/)
2. Sign in with your GitHub account
3. Click **"File" → "Add Local Repository"**
4. Select your project folder
5. Click **"Publish repository"** to upload to GitHub

## License

This project is private and proprietary.

## Support

For issues or questions, please check the project repository or contact the development team.

