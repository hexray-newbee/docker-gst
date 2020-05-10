FROM dyhexl/gst-dev:1.16.2

RUN echo 'export RUSTUP_DIST_SERVER=https://mirrors.tuna.tsinghua.edu.cn/rustup' >> ~/.bash_profile && \
  curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y

RUN apt-get update && \
  apt-get install -y \
  python3-pip \
  ninja-build

RUN pip3 install -i https://mirrors.aliyun.com/pypi/simple pip -U && \
  pip3 config set global.index-url https://mirrors.aliyun.com/pypi/simple

RUN pip3 install meson

RUN apt-get update && \
  apt-get install -y \
  cargo

RUN apt-get update && \
  apt-get install -y \
  libssl-dev

# remove all package lists
RUN rm -rf /var/lib/apt/lists/*
