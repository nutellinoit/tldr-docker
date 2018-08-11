FROM node:8.11.3-alpine
RUN apk update && \
    apk upgrade && \
    apk add git
RUN apk add python make g++
ADD rootfs /rootfs
WORKDIR /rootfs
RUN rm .git
RUN git init
RUN npm install -g --unsafe-perm
RUN apk del python make g++
ENTRYPOINT ["tldr"]
CMD ["--help"]