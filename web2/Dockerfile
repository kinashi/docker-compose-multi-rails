FROM ruby:2.3.1
RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs
RUN mkdir /web2
WORKDIR /web2
ADD Gemfile /web2/Gemfile
ADD Gemfile.lock /web2/Gemfile.lock
RUN bundle install
ADD . /web2