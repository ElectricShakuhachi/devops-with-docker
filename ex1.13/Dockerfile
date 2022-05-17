FROM golang:1.16
COPY . .
RUN rm go.mod
COPY . ..
RUN cd ..; go build
CMD ../server