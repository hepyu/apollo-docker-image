# Dockerfile for apollo-portal-server

# Build with:
# docker build -t apollo-portal-server:v1.0.0 .

FROM hpy253215039/oraclejdk-skywalking-linux-64:8u221
RUN mkdir -p /apollo-portal-server

ADD . /apollo-portal-server/

ENV APOLLO_PORTAL_SERVICE_NAME="service-apollo-portal-server.sre"

EXPOSE 8070

CMD ["/apollo-portal-server/scripts/startup-kubernetes.sh"]
