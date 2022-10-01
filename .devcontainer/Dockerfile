FROM fedora:36

RUN echo 'max_parallel_downloads=20' | tee -a /etc/dnf/dnf.conf \
    && dnf update --refresh -y \
    && dnf install -y vim htop fish git curl cmake ninja-build meson clang \
    && useradd --create-home -s /bin/fish rajveer \
    && echo "rajveer ALL=(root) NOPASSWD:ALL" > /etc/sudoers.d/rajveer
