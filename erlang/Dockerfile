FROM ghcr.io/rotespferd/devcontainer/base:39

ARG ERLANG_VERSION=26.2.2

RUN wget https://packages.erlang-solutions.com/erlang-solutions-2.0-1.noarch.rpm && \
    rpm -Uvh erlang-solutions-2.0-1.noarch.rpm

RUN dnf -y install erlang-${ERLANG_VERSION} && dnf clean all