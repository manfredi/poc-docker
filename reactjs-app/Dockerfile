# docker build --no-cache -t poc-reactjs-app:latest .
# docker run -d --name poc-reactjs-app --rm -p 9000:3000 poc-reactjs-app:latest

FROM node:current-buster-slim
WORKDIR /app
USER root
RUN apt update && apt install -y git
RUN git clone -b master --depth 1 https://github.com/Rahul-Pandey7/react-image-compressor.git .
ENV PATH /app/node_modules/.bin:$PATH
RUN npm install -g npm@latest
RUN npm install
EXPOSE 3000
CMD ["npm", "start"]
