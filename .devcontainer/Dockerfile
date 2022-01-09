ARG VARIANT=2.5
FROM mcr.microsoft.com/vscode/devcontainers/ruby:0-${VARIANT}

ENV NODE_VERSION="12"
ENV RAILS_DEVELOPMENT_HOSTS=".githubpreview.dev"

RUN curl -sL https://deb.nodesource.com/setup_${NODE_VERSION}.x | bash - \
  && apt-get update \
  && apt-get -y install git procps nodejs

RUN gem install bundler

WORKDIR /usr/src/app
COPY ./Gemfile ./Gemfile.lock ./
RUN bundle install

EXPOSE 3000
