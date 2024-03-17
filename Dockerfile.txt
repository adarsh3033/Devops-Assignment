FROM golang:1.16-alpine

WORKDIR /app
COPY . .

RUN go build -o myapp

EXPOSE 8080
CMD ["./myapp"]
