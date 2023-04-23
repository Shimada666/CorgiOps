FROM node:14-slim

ENV NPM_REGISTRY https://registry.npmmirror.com

RUN sed -i 's#http://deb.debian.org#http://mirrors.bfsu.edu.cn#g' /etc/apt/sources.list && \
    apt update

RUN npm config set registry $NPM_REGISTRY
RUN npm install -g pnpm@7

CMD ["bash"]