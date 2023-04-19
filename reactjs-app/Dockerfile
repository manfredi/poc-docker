# docker build --no-cache -t poc-reactjs-app:latest .
# docker run -d --name poc-reactjs-app --rm -p 9000:3000 poc-reactjs-app:latest

FROM node:alpine3.17
WORKDIR /app
USER root
RUN apk add git
RUN git clone -b main --depth 1 https://github.com/springheart199279/web-developer-tools.git .
ENV PATH /app/node_modules/.bin:$PATH
RUN npm install
EXPOSE 3000
CMD ["npm", "start"]
