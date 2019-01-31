FROM node:10.15.0-alpine
RUN npm install -g @vue/cli &&  npm install -g @vue/cli-init && npm install -g @vue/cli-service
WORKDIR /usr/src/app/client/
COPY app/client/. .
RUN npm install && npm cache clean --force
VOLUME /usr/src/app/client/
EXPOSE 8080