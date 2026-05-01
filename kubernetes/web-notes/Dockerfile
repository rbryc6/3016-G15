FROM node:latest
RUN mkdir -p /usr/local/app
WORKDIR /usr/local/app
RUN git clone https://github.com/AloisCRR/notes-web-app /usr/local/app
ENV WEB_APP_NOTES_MONGODB_HOST="172.17.0.2:27017"
ENV WEB_APP_NOTES_MONGODB_DATABASE="web-notes"
RUN npm install
RUN npm install handlebars@4.5.3
CMD ["npm","run","dev"]
EXPOSE 4000
