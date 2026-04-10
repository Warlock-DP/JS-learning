# JavaScript Development Environment Setup

This workspace is configured with Node.js and JavaScript development tools.

## Configuration Files Created

1. **devcontainer.json** - VS Code dev container configuration with Node.js 20
2. **Dockerfile** - Custom Docker image for JavaScript development
3. **docker-compose.yml** - Docker Compose configuration for easy container management

## How to Use

### Option 1: VS Code Dev Container (Recommended)
1. Install the "Dev Containers" extension in VS Code
2. Click on the `><` icon in the bottom-left corner
3. Select "Reopen in Container"
4. VS Code will build and start the container with Node.js and all tools

### Option 2: Manual Installation (Ubuntu)
If you prefer to install Node.js directly on your system:

```bash
sudo apt update
sudo apt install -y nodejs npm
```

### Option 3: Using Docker Compose
```bash
docker-compose up -d
docker-compose exec js-learning bash
```

## Included Tools & Extensions

- **Node.js 20** with npm
- **Git & GitHub CLI** for version control
- **VS Code Extensions:**
  - ESLint - Code quality
  - Prettier - Code formatting
  - JS Debugger - JavaScript debugging
  - Live Server - Local development server

## Common Commands

```bash
# Check Node.js and npm versions
node --version
npm --version

# Initialize a new project
npm init -y

# Install dependencies
npm install <package-name>

# Run a development server
npm start

# Run ESLint
npx eslint .

# Format with Prettier
npx prettier --write .
```

## Project Structure

Once set up, you can create JavaScript projects in this workspace:

```
JS-learning/
├── .devcontainer/        # Dev container config
├── .git/                 # Git repository
├── README.md
└── src/                  # Your JavaScript source files
    └── index.js
```

## Next Steps

1. Restart VS Code or reopen the folder in a container
2. Create a `package.json` if you need to manage dependencies
3. Start building your JavaScript projects!
