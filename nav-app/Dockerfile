# Build stage

FROM node:latest 

WORKDIR /nav-app/

# copy over needed files
COPY . ./

RUN npm run build

RUN npm install http-server -g

WORKDIR /nav-app/dist/

EXPOSE 4200

CMD http-server -a 0.0.0.0 -p 4200
