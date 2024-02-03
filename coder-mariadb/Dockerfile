FROM ghcr.io/eve0415/coder-node

USER root
RUN apt-get update && apt-get upgrade -y \
    && apt-get install mariadb-server --no-install-recommends -y \
    && apt-get autoremove --purge -y && rm -rf /var/lib/apt/lists/*

USER node
RUN code-server --install-extension Prisma.prisma
