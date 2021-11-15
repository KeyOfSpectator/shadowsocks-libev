#
# Dockerfile for shadowsocks-libev
#

FROM shadowsocks/shadowsocks-libev
LABEL maintainer="KeyOfSpectator <413070456@qq.com>"

USER root
ENV PLUGIN /v2ray-plugin_linux_amd64
ENV PLUGIN_OPTS server

COPY ./v2ray-plugin_linux_amd64 /v2ray-plugin_linux_amd64
RUN chmod 755 /v2ray-plugin_linux_amd64

USER nobody

COPY ./entrypoint.sh /entrypoint.sh

CMD /entrypoint.sh
