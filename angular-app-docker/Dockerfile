FROM node:14.15.5-alpine3.10
RUN npm install -g @angular/cli@11.2.12
RUN addgroup app && adduser -S -G app app
USER app
WORKDIR /app
#RUN mkdir data
COPY package*.json ./
RUN npm install
COPY . .
ENV API_PATH=http://localhost
EXPOSE 4200
RUN npm run build
ENTRYPOINT ["ng", "serve", "--host", "0.0.0.0", "--disable-host-check", "--poll", "20"]