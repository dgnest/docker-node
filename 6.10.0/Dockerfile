FROM node:6.10.0
MAINTAINER Luis Mayta <@slovacus>

# Install OptiPNG
ONBUILD RUN export LANG=C.UTF-8 && \
            apt-get update -y && \
            apt-get install -y optipng \
            ruby ruby-dev && \
            gem install bundle && \
            npm install --global gulp-cli