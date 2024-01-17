## OpenSearch PoC

A lightweight PoC to demonstrate OpenSearch capabilities for logging with:
- vector (Logstash/Fluentd/Fluentbit alternative) as centralized analyser;
- redpanda (Kafka) as stream for durability;

**Use cases:**
1. Collect access and app logs (tomcat, apache httpd, nagios)
2. Collect network packet data (DNS, HTTP, ICMP, etc.) (packetbeat)
3. Collect server metrics (metricbeat)

**Transformations:**
1. Multiple parsing strategies: parsing syslog, common log, and regex for niche technologies.
2. Redact sensitive data by using regex.
3. SHA-3 hashing via "sha3"
4. Enrich data with GeoIP data.

