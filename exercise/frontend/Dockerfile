FROM node:18
WORKDIR /app
COPY . .
RUN npm install -g npm@latest
RUN npm cache clean --force
RUN npm install
ENV PORT=8000
EXPOSE 8000
ENV REACT_APP_BACKEND_URL=http://backend:8001
VOLUME [ "/frontend-app" ]
CMD ["npm", "start"]
