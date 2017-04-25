FROM node:6.10.0
MAINTAINER Luis Mayta <@slovacus>

# Install OptiPNG
RUN export LANG=C.UTF-8 \
          && apt-get update -y \
          && apt-get install -y optipng \
          zlib1g-dev build-essential libssl-dev \
          libreadline-dev libyaml-dev \
          libsqlite3-dev sqlite3 libxml2-dev \
          libxslt1-dev libcurl4-openssl-dev \
          libffi-dev \
          && wget http://ftp.ruby-lang.org/pub/ruby/2.3/ruby-2.3.3.tar.gz \
          && tar -xzvf ruby-2.3.3.tar.gz \
          && cd ruby-2.3.3/ \
          && ./configure \
          && make \
          && make install \
          && cd .. \
          && rm -rf ruby-2.3.3.tar.gz \
          && rm -rf ruby-2.3.3 \
          && gem install bundle \
          && apt-get autoclean \
          && apt-get autoremove \
          && rm -rf /var/lib/apt/lists/*