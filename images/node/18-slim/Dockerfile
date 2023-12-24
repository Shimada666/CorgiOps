FROM node:18-slim

ENV NPM_REGISTRY https://registry.npmmirror.com

RUN sed -i 's#http://deb.debian.org#http://mirrors.bfsu.edu.cn#g' /etc/apt/sources.list.d/debian.sources && apt update

RUN npm config set registry $NPM_REGISTRY
RUN npm install -g pnpm

CMD ["bash"]