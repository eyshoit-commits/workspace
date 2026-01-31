FROM mcr.microsoft.com/devcontainers/javascript-node:latest

# Install Bun
RUN curl -fsSL https://bun.sh/install | bash

# Install pnpm
RUN corepack enable && corepack prepare pnpm@latest --activate

# Install other dependencies if needed
