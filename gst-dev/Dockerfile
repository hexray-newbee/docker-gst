FROM dyhexl/gst-launch:1.16.2

RUN apt-get update && \
  apt-get install -y \
  libgstreamer1.0-dev \
  libgstreamer-plugins-base1.0-dev \
  libgstreamer-plugins-good1.0-dev \
  libgstreamer-plugins-bad1.0-dev

# remove all package lists
RUN rm -rf /var/lib/apt/lists/*
