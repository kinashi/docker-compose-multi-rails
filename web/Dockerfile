FROM ruby:2.3.1
RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs
RUN mkdir /web
WORKDIR /web
ADD Gemfile /web/Gemfile
ADD Gemfile.lock /web/Gemfile.lock
RUN bundle install
ADD . /web