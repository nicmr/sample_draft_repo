FROM rust:1.19.0

USER runner
WORKDIR /usr/src/app
COPY . /usr/src/app
RUN cargo install && cargo build

ENV PORT 8080
EXPOSE 8080

CMD ["cargo", "run", "-q"]
