FROM clearlinux:base

RUN groupadd --gid 1000 vscode \
    && useradd --uid 1000 --gid vscode -m vscode \
    && echo "vscode ALL=(root) NOPASSWD:ALL" > /etc/sudoers.d/vscode
