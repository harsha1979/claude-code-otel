FROM grafana/grafana-oss:latest

COPY grafana-datasources.yml /etc/grafana/provisioning/datasources/datasources.yml
COPY grafana-dashboards.yml /etc/grafana/provisioning/dashboards/dashboards.yml
COPY claude-code-dashboard.json /var/lib/grafana/dashboards/claude-code-dashboard.json

USER 10014