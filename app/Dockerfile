FROM ruby:latest

ENV USER=rubyuser
ENV UID=12345
ENV GID=23456

#    --disabled-password prevents prompt for a password
#    --gecos "" circumvents the prompt for "Full Name" etc. on Debian-based systems
RUN adduser \
    --disabled-password \
    --gecos "" \
    --uid "$UID" \
    "$USER"

# ensures "rootless" approach
USER $USER

WORKDIR /home/$USER

# get app code in-line - cause it could be changed with time
RUN curl -o webserver.rb https://raw.githubusercontent.com/sawasy/http_server/main/http_server.rb

RUN bundle init

EXPOSE 80

CMD ["ruby", "/home/rubyuser/webserver.rb"]
