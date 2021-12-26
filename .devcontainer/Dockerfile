FROM ubuntu:20.04

RUN apt update \
    && apt install -y make cmake curl wget \
    && apt install -y gcc g++ git

RUN apt install -y software-properties-common
RUN add-apt-repository -y ppa:ethereum/ethereum
RUN apt update
RUN apt install -y ethereum
# https://geth.ethereum.org/docs/install-and-build/installing-geth#install-on-ubuntu-via-ppas
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -s -- -y
RUN apt install -y nodejs
RUN npm config set unsafe-perm true
RUN npm install -g truffle
RUN npm install ganache-cli@latest --global
RUN npm install ganache
RUN npm install openzeppelin-solidity
