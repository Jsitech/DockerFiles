# Run Joomla Vulnerability Scanner in a Docker Container
#
#
# A black box, Ruby powered, Joomla vulnerability scanner

FROM ruby:2.2

MAINTAINER Jason Soto "jason_soto@jsitech.com"

ENV DEBIAN_FRONTEND noninteractive

# Clone Project Repo

RUN git clone https://github.com/rastating/joomlavs

WORKDIR joomlavs/

RUN bundle install

ENTRYPOINT ["ruby","joomlavs.rb"]
