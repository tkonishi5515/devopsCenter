FROM ubuntu:22.04.2 LTS

RUN apt-get update && \
    apt-get install -y \
      libx11-xcb \
      libxrandr \
      libxcb \
      libxcomposite \
      libxcursor \
      libxdamage \
      libxfixes \
      libxi \
      libxrender \
      libxss \
      libxtst \
      libnss3 \
      libnspr4 \
      libatk1.0-0 \
      libatspi2.0-0 \
      libgdk-pixbuf2.0-0 \
      libgtk-3-0 \
      libpango-1.0-0 \
      libcairo2 \
      libxcomposite \
      xkb-data \
      libxshmfence1 && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*
