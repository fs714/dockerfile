FROM ubuntu:16.04

MAINTAINER fs714 <fs714@163.com>

ENV HOME /root
ENV PYENV_ROOT $HOME/.pyenv
ENV PATH $PYENV_ROOT/shims:$PYENV_ROOT/bin:$PATH

WORKDIR /root

RUN apt-get update && \
    apt-get install -y wget curl && \
    apt-get install -y --no-install-recommends make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev llvm libncurses5-dev xz-utils tk-dev git vim && \
    rm -rf /var/lib/apt/lists/* && \
    git clone git://github.com/yyuu/pyenv.git .pyenv && \
    pyenv install 3.6.0 && \
    pyenv global 3.6.0 && \
    pyenv rehash

CMD ["bash"]
