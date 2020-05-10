FROM dyhexl/gst-launch:1.16.2

RUN apt-get update && \
  apt-get install -y \
  nodejs

# remove all package lists
RUN rm -rf /var/lib/apt/lists/*
