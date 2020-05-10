FROM dyhexl/gst-launch:1.16.2

RUN apt-get update && \
  apt-get install -y \
  libgstreamer1.0-dev \
  libgstreamer-plugins-base1.0-dev \
  libgstreamer-plugins-good1.0-dev \
  libgstreamer-plugins-bad1.0-dev

RUN apt-get update && \
  apt-get install -y \
  python3-pip \
  ninja-build && \
  pip3 install -i https://mirrors.aliyun.com/pypi/simple pip -U && \
  pip3 config set global.index-url https://mirrors.aliyun.com/pypi/simple && \
  pip3 install meson

RUN apt-get update && \
  apt-get install -y \
  git \
  gdb

# remove all package lists
RUN rm -rf /var/lib/apt/lists/*
