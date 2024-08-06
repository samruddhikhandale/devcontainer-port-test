# Make sure RUBY_VERSION matches the Ruby version in .ruby-version
ARG RUBY_VERSION=3.2.2
FROM ghcr.io/rails/devcontainer/images/ruby:$RUBY_VERSION

RUN apt-get update -qq && \
    apt-get install --no-install-recommends -y curl libjemalloc2 default-libmysqlclient-dev libvips \
      git node-gyp pkg-config python-is-python3 autoconf automake libtool && \
      rm -rf /var/lib/apt/lists /var/cache/apt/archives
