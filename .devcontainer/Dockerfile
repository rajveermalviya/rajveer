FROM fedora:36

RUN echo 'max_parallel_downloads=20' | tee -a /etc/dnf/dnf.conf \
    && dnf update --refresh -y \
    && dnf install -y vim htop fish git curl cmake ninja-build meson clang \
    && groupadd --gid 1000 vscode \
    && useradd -s /bin/fish --uid 1000 --gid vscode -m vscode \
