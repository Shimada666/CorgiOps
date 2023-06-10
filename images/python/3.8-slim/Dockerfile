FROM python:3.8-slim

RUN pip config set global.index-url https://mirrors.bfsu.edu.cn/pypi/web/simple && \
    pip config set install.trusted-host mirrors.bfsu.edu.cn

RUN sed -i 's#http://deb.debian.org#https://mirrors.ustc.edu.cn#g' /etc/apt/sources.list && \
    sed -i 's|security.debian.org/debian-security|mirrors.ustc.edu.cn/debian-security|g' /etc/apt/sources.list && \
    apt update

