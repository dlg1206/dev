# Dev Alpine Image
FROM alpine:3.22 AS runtime
LABEL maintainer="Derek Garcia <dgarcia2@hawaii.edu>"
LABEL alpine_version=3.22
LABEL name=alpine-dev
# copy config files
COPY dotfiles/gitconfig/.gitconfig dotfiles/vimrc/.vimrc images/alpine/.profile /root/
# add util tools
RUN apk add --no-cache curl vim jq git
# launch shell
WORKDIR /dev
ENTRYPOINT ["ash", "--login"]