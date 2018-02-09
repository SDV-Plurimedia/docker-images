FROM alpine:edge

RUN apk --no-cache --repository http://dl-3.alpinelinux.org/alpine/edge/testing/ add \
 nodejs nodejs-npm chromium firefox xwininfo xvfb dbus eudev ttf-freefont fluxbox

RUN npm install -g testcafe && \
 npm cache clean && \
 rm -rf /tmp/* && \
 adduser -D user

USER user
ENTRYPOINT ["/bin/sh", "-c"]

