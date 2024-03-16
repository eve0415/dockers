FROM mcr.microsoft.com/devcontainers/typescript-node:1-20-bookworm
RUN curl -fsSL https://code-server.dev/install.sh | sh
RUN corepack enable yarn pnpm

USER node
RUN code-server --install-extension esbenp.prettier-vscode && \
    code-server --install-extension dbaeumer.vscode-eslint && \
    code-server --install-extension biomejs.biome && \
    code-server --install-extension ambar.bundle-size && \
    code-server --install-extension mhutchie.git-graph && \
    code-server --install-extension ms-azuretools.vscode-docker && \
    code-server --install-extension github.vscode-github-actions && \
    code-server --install-extension GitHub.vscode-pull-request-github
