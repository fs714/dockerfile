FROM ubuntu:16.04

MAINTAINER fs714 <fs714@163.com>

RUN apt update
RUN apt install -y make build-essential python-dev libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev libncursesw5-dev git

WORKDIR /root

RUN git clone git://github.com/yyuu/pyenv.git .pyenv

ENV HOME /root
ENV PYENV_ROOT $HOME/.pyenv
ENV PATH $PYENV_ROOT/shims:$PYENV_ROOT/bin:$PATH

RUN \
    pyenv install 3.6.0 && \
    pyenv global 3.6.0 && \
    pyenv rehash

CMD ["bash"]
