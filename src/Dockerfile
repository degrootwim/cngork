FROM node

LABEL maintainer Wim de Groot

RUN npm install ngrok -g

ENV AUTH_TOKEN=example
ENV PROTOCOL=http
ENV SUBDOMAIN=subdomain
ENV REGION=eu
ENV ADDRESS=localhost

ENTRYPOINT ngrok authtoken ${AUTH_TOKEN} \
            && ngrok ${PROTOCOL} ${ADDRESS} \
            -subdomain ${SUBDOMAIN} \
            -region ${REGION}