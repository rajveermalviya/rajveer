FROM fedora:38

RUN echo 'max_parallel_downloads=20' | tee -a /etc/dnf/dnf.conf \
    && dnf update --refresh -y \
    && dnf install -y vim htop fish git curl cmake ninja-build meson clang \
    && useradd -m -r -s /usr/bin/fish -u 1000 -U vscode \
    && echo "vscode ALL=(root) NOPASSWD:ALL" > /etc/sudoers.d/vscode
