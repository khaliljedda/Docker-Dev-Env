FROM node:13-alpine                
WORKDIR /app
COPY package.json ./
RUN  npm install -g @angular/cli@^9.1.15
RUN  npm install
EXPOSE 4200
CMD ["ng","serve","--host", "0.0.0.0"]

