

FROM grafana/grafana:13.3.0

# Grafana Netzwerk
ENV GF_SERVER_HTTP_ADDR=0.0.0.0 \
    GF_SERVER_HTTP_PORT=3000

# Benutzerverwaltung
ENV GF_USERS_ALLOW_SIGN_UP=false \
    GF_AUTH_ANONYMOUS_ENABLED=false

# Keine automatischen externen Updates
ENV GF_ANALYTICS_REPORTING_ENABLED=false \
    GF_ANALYTICS_CHECK_FOR_UPDATES=false \
    GF_ANALYTICS_CHECK_FOR_PLUGIN_UPDATES=false \
    GF_PLUGINS_PREINSTALL_AUTO_UPDATE=false

# Build abbrechen, falls InfluxDB nicht enthalten ist
RUN test -f /usr/share/grafana/data/plugins-bundled/influxdb/plugin.json

EXPOSE 3000
