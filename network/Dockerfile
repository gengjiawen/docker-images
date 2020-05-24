FROM gengjiawen/node-build

ENV PATH="/root/.cargo/bin:${PATH}"
RUN curl  https://sh.rustup.rs -sSf | sh -s --  -y
RUN apt install sudo net-tools iputils-ping iproute2 -y
RUN cd /tmp && git clone https://github.com/gengjiawen/network-demo && \
    cd network-demo/tcp && cargo build --release