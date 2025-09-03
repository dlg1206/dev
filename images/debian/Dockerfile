# Dev Debian Image
FROM debian:bookworm-slim AS runtime
LABEL maintainer="Derek Garcia <dgarcia2@hawaii.edu>"
LABEL debian_version=12
LABEL name=debin-dev
# add util tools
RUN apt update \
    && apt install -y curl vim jq git iputils-ping \
    && rm -rf /var/lib/apt/lists/*
# copy config files
COPY dotfiles/gitconfig/.gitconfig dotfiles/vimrc/.vimrc images/debian/.profile /root/
# launch shell
WORKDIR /dev
ENTRYPOINT ["bash", "--login"]