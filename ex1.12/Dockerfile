FROM ubuntu:20.04
COPY . .
RUN apt update
RUN apt install -y curl
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash
RUN apt install -y nodejs
RUN npm install
RUN npm run build
RUN npm install -g serve
CMD serve -s -l 5000 build