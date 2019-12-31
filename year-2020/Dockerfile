FROM alpine:latest AS builder
COPY . .

FROM scratch
COPY --from=builder . .
ENTRYPOINT [ "cat", "doodle.txt" ]