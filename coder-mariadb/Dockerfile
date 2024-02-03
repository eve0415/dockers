FROM ghcr.io/eve0415/coder-node
RUN apt-get update && apt-get upgrade -y \
    && apt-get install mariadb-server --no-install-recommends -y \
    && apt-get autoremove --purge -y && rm -rf /var/lib/apt/lists/*
RUN code-server --install-extension Prisma.prisma
