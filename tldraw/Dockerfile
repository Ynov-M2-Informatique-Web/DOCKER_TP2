FROM node:14-alpine

RUN apk add --no-cache git
WORKDIR /app
RUN git clone --depth 1 --branch main https://github.com/tldraw/tldraw-examples.git .
RUN yarn install

EXPOSE 5173

CMD ["yarn", "dev", "--host", "0.0.0.0"]