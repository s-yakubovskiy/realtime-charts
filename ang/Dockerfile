FROM node:latest
RUN apt update && apt install -y vim
RUN npm install -g @angular/cli
COPY ./ang/RealTime_client /app
WORKDIR /app
RUN npm install; exit 0
CMD ["/usr/local/bin/ng", "serve", "--host", "0.0.0.0"]
