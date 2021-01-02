FROM ruby:3.0
RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs
WORKDIR /app/api
ADD Gemfile /app/api/Gemfile
ADD Gemfile.lock /app/api/Gemfile.lock
RUN bundle install
ADD . /app/api