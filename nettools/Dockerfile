FROM ubuntu:24.04
# Any Dockerfile MUST initialize with the FROM statement.

LABEL author="Ronald Bulbow" \
      creation_date="Dec/02/2024" \
      description="Provide Network Tools for troubleshooting"

USER root

SHELL [ "/usr/bin/bash", "-c" ]
ENV SHELL=/usr/bin/bash

RUN <<EOF
apt update
apt install -y elinks vim nano bash net-tools coreutils curl wget iperf3 iproute2 iptables keepalived \
  nftables socat netcat-openbsd ethtool mtr tcpdump lshw nmap bind9-dnsutils busybox iputils-arping iputils-ping \
  iputils-tracepath iptables
apt autoclean
apt autoremove
EOF

CMD ["bash"]

