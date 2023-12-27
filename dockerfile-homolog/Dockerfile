FROM node

WORKDIR /usr/app

RUN apt-get update && apt-get install -y git

RUN git clone -b homolog --single-branch https://github.com/hari6091/backend-ingress.git

WORKDIR /usr/app/backend-ingress

EXPOSE 5000

CMD ["sh", "-c", "git pull && npm install && npm run start"]
