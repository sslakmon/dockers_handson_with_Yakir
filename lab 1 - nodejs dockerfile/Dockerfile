FROM node:20

WORKDIR /app/src/app

#  copy nodjs configuration file so the npm install will install all the dependecies 
COPY ./package.json .
# install express based on the dependencies in the package.json
RUN npm install express 

EXPOSE 3000
# copy from my curren out of container folde to my current folder inside th econtainer 
COPY . .

CMD ["node","server.js"]

