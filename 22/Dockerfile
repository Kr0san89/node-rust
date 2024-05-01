FROM node:22

# get dependencies
RUN apt-get update && apt-get install -y curl wget && apt-get clean

#install rust
RUN RUSTUP_URL="https://sh.rustup.rs" \
  && curl --silent --show-error --location --fail --retry 1 --proto '=https' --tlsv1.2 --output /tmp/rustup-linux-install.sh $RUSTUP_URL \
  && bash /tmp/rustup-linux-install.sh -y \
  && rm /tmp/rustup-linux-install.sh

RUN find / -name rustup
  
# add windows target
RUN ${HOME}/.cargo/bin/rustup target add x86_64-pc-windows-msvc

ENV PATH /root/.cargo/bin:${PATH}  

# get versions
CMD rustc --version && echo -n "Node:"; node --version
