FROM ubuntu:bionic

ENV HOME /root

WORKDIR /root

RUN \
    apt update && \
    apt -y upgrade && \
    apt install -y git curl make man unzip vim wget gcc valgrind zsh && \
    rm -rf /var/lib/apt/lists/* && \
    git clone https://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh && \
    cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc

CMD ["zsh"]