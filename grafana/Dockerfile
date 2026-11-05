
# Grafana fuer IXON SecureEdge Pro
# ARM64 / Grafana OSS 13.3.0
#
# Saubere Installation ohne zusaetzliche Plugins.
# Keine fest eingebauten Passwoerter oder Tokens.
# InfluxDB wird spaeter in Grafana konfiguriert.

FROM grafana/grafana:13.3.0-slim

ENV GF_SERVER_HTTP_ADDR=0.0.0.0 \
    GF_SERVER_HTTP_PORT=3000 \
    GF_USERS_ALLOW_SIGN_UP=false \
    GF_AUTH_ANONYMOUS_ENABLED=false \
    GF_ANALYTICS_REPORTING_ENABLED=false \
    GF_ANALYTICS_CHECK_FOR_UPDATES=false \
    GF_ANALYTICS_CHECK_FOR_PLUGIN_UPDATES=false

EXPOSE 3000

