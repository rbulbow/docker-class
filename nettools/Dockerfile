FROM ubuntu:24.04
# Any Dockerfile MUST initialize with the FROM statement.

LABEL author="Ronald Bulbow" \
      creation_date="Dec/02/2024" \
      description="Provide Network Tools for troubleshooting"

USER root

RUN <<EOF
apt update
apt -y upgrade
apt -y install elinks vim nano bash net-tools conntrack-tools coreutils curl wget \
       drill iperf3 iproute2 iptables iputils ip6tables keepalived nftables socat \
       bind-tools nc ethtool mtr tcpdump lshw nmap busybox-extras
apt autoclean
apt autoremove
EOF

CMD bash


