FROM node:19-alpine
RUN apk add --no-cache chromium
ENV PUPPETEER_SKIP_CHROMIUM_DOWNLOAD="true"
WORKDIR /app
RUN chown node:node /app
COPY --chown=node:node . .
USER node
RUN npm install
CMD npm run start
