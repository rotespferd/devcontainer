# Argument for specifying the PHP version
ARG FEDORA_VERSION

FROM fedora:${FEDORA_VERSION}

RUN dnf -y update

# Install base packages
RUN dnf install -y git unzip zip wget curl