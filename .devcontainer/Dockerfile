FROM mcr.microsoft.com/devcontainers/javascript-node:1-22-bookworm

# Keep package metadata fresh for interactive apt usage in the container.
RUN apt-get update \
	&& apt-get install -y --no-install-recommends ca-certificates ripgrep \
	&& rm -rf /var/lib/apt/lists/*
