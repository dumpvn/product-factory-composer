FROM docker.io/envoyproxy/envoy-dev:latest

COPY docker-compose/proxy/envoy.yaml /etc/envoy.yaml
RUN chmod go+r /etc/envoy.yaml
CMD ["/usr/local/bin/envoy", "-c /etc/envoy.yaml", "-l", "debug"]
