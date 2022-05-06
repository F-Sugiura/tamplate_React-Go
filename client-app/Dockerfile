FROM node:18-alpine3.15
ENV NODE_VERSION 16.15.0
WORKDIR /home/client-app
COPY ["./package.json", "./yarn.lock"]
RUN yarn --frozen-lockfile --silent
COPY [".", "./"]
RUN yarn build
CMD ["yarn", "start"]
