FROM prom/prometheus:latest

COPY prometheus.yml /etc/prometheus/prometheus.yml

# Choreo runtime can mount /prometheus with different ownership.
# Use writable /tmp paths to avoid permission-denied on queries.active.
CMD ["--config.file=/etc/prometheus/prometheus.yml", "--storage.tsdb.path=/tmp/prometheus", "--query.active-query-tracker-dir=/tmp/prometheus"]

USER 10014