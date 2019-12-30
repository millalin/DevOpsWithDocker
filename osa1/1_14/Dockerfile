
FROM ruby:2.6.0

EXPOSE 3000
COPY ./rails-example-project /usr/ex14
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
WORKDIR /usr/ex14
RUN gem install bundler
RUN bundle install
RUN rails db:migrate
CMD rails s

