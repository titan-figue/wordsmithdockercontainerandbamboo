FROM golang
WORKDIR /dispatcher/
COPY dispatcher.go .
COPY ./static/ ./static
RUN go build dispatcher.go
CMD ./dispatcher
EXPOSE 80