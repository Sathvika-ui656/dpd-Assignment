FROM golang:1.23 as builder

WORKDIR /app

COPY . .

RUN go build -o service1 main.go

FROM debian:bookworm-slim

WORKDIR /app

COPY --from=builder /app/service1 .

EXPOSE 8001

CMD ["./service1"]
