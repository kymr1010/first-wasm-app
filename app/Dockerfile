FROM rust:1.61.0

WORKDIR /usr/src/app
COPY . .

RUN cargo install wasm-pack

RUN apt update && apt install -y curl
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash
RUN apt install -y nodejs

EXPOSE 8080

CMD ["bash"]