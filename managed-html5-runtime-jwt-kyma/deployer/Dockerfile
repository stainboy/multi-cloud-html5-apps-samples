FROM node:16-alpine

RUN mkdir -p /app && \
    chown node.node /app

# Create app directory
WORKDIR /app

# Bundle app source
COPY . .
RUN npm install  --production

EXPOSE 5000
CMD [ "npm", "start" ]

# docker build -t eureka-docker-prod.common.repositories.cloud.sap/eureka/kyma-simple-backend:dev .
