FROM ubuntu:16.04
WORKDIR /mydir
RUN apt-get update && apt-get install -y curl && apt-get install -y apt-utils
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt-get install -y nodejs
COPY . .
RUN npm install
EXPOSE 5000
CMD ["npm", "start"]