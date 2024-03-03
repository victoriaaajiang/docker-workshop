FROM node:18
WORKDIR /backend-app
COPY . .
RUN npm install -g npm@latest
RUN npm cache clean --force
RUN npm install
ENV PORT=8001
EXPOSE 8001
VOLUME [ "/backend-app" ]
CMD ["node", "index.js"]
