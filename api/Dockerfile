FROM ruby:2.6.3

WORKDIR /app
COPY Gemfile /app
COPY Gemfile.lock /app
COPY . /app

RUN apt-get update -qq && apt-get install -y build-essential nodejs libpq-dev postgresql-client
RUN gem update bundler && bundle install
