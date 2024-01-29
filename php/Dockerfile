# Set the base image to Fedora
FROM fedora:39

# Argument for specifying the PHP version
ARG PHP_VERSION

# Install PHP
RUN dnf -y update

RUN dnf install -y https://rpms.remirepo.net/fedora/remi-release-$(rpm -E %fedora).rpm && \
    sudo dnf module reset php && \
    sudo dnf module enable -y php:remi-${PHP_VERSION} && \
    sudo dnf install -y php

# Install Composer

# Define the entry point script
ENTRYPOINT ["php", "-a"]