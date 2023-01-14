FROM nginx:alpine

RUN apk add git
COPY nginx.conf /etc/nginx/conf.d/default.conf
RUN git clone https://we.phorge.it/source/arcanist.git /arcanist
