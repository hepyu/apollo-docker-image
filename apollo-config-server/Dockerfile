# Dockerfile for apollo-config-server

# Build with:
# docker build -t apollo-config-server:v1.0.0 .

FROM hpy253215039/oraclejdk-skywalking-linux-64:8u221
RUN mkdir -p /apollo-config-server

ADD . /apollo-config-server/

ENV APOLLO_CONFIG_SERVICE_NAME="service-apollo-config-server.sre"

EXPOSE 8080

CMD ["/apollo-config-server/scripts/startup-kubernetes.sh"]
