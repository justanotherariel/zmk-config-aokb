FROM zmkfirmware/zmk-build-arm:stable

# Modify existing ubuntu user (UID 1000) to have GID 100
RUN usermod -g 100 ubuntu

# Install additional tools
RUN apt-get update && \
    apt-get install -y just yq bsdmainutils fzf && \
    rm -rf /var/lib/apt/lists/*

# Set the default user
USER ubuntu
