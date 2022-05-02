FROM fedora:36
USER rajveer
COPY library-scripts/common-fedora.sh /tmp/library-scripts/
RUN bash /tmp/library-scripts/common-fedora.sh
RUN useradd --create-home -s /bin/bash rajveer && \
        echo "rajveer ALL=(root) NOPASSWD:ALL" > /etc/sudoers.d/rajveer
