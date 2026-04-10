FROM node:20-ubuntu

# Install essential tools
RUN apt-get update && apt-get install -y \
    git \
    curl \
    wget \
    build-essential \
    python3 \
    && rm -rf /var/lib/apt/lists/*

# Update npm to the latest version
RUN npm install -g npm@latest

# Set working directory
WORKDIR /workspaces/JS-learning

# Copy package files if they exist
COPY package*.json ./

# Install dependencies if package.json exists
RUN if [ -f package.json ]; then npm install; fi

# Expose port for development servers
EXPOSE 3000 5500 8080

CMD ["/bin/bash"]
