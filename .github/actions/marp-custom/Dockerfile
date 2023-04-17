FROM marpteam/marp-cli:latest

# Install Puppeteer dependencies
RUN echo 'deb http://deb.debian.org/debian/ stretch main' > /etc/apt/sources.list.d/stretch.list \
 && apt-get update \
 && apt-get install -y --no-install-recommends \
      libx11-xcb1 \
      libxrandr2 \
      libxcb1 \
      libxcomposite1 \
      libxcursor1 \
      libxdamage1 \
      libxfixes3 \
      libxi6 \
      libxrender1 \
      libxss1 \
      libxtst6 \
      libnss3 \
      libnspr4 \
      libatk1.0-0 \
      libatk-bridge2.0-0 \
      libatspi2.0-0 \
      libgdk-pixbuf2.0-0 \
      libgtk-3-0 \
      libpango-1.0-0 \
      libpangocairo-1.0-0 \
      libxcomposite1 \
      libxkbcommon0 \
      libxshmfence1 \
 && apt-get clean \
 && rm -rf /var/lib/apt/lists/*
