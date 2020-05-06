FROM dyhexl/gst-launch:1.16.2

RUN apt-get update && \
  apt-get install -y \
  python3-pip \
  gir1.2-gst* \
  python3-gst-1.0

RUN pip3 install -i https://mirrors.aliyun.com/pypi/simple pip -U && \
  pip3 config set global.index-url https://mirrors.aliyun.com/pypi/simple

# remove all package lists
RUN rm -rf /var/lib/apt/lists/*
