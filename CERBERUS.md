# Cerberus fork notes

This branch (`cerberus-ddl`) of github.com/open-telemetry/opentelemetry-collector-contrib
exposes the OTel ClickHouse Exporter's SQL templates by moving
`exporter/clickhouseexporter/internal/sqltemplates/` out of `internal/`,
so [github.com/tsouza/cerberus](https://github.com/tsouza/cerberus) can
import the canonical schema DDL as the source-of-truth for its tests
and runtime auto-create path.

Each commit is a single mechanical move/rename so the patch can be
reviewed in isolation (and is a candidate for an upstream PR if OTel
maintainers want to upstream the export).

Upstream: https://github.com/open-telemetry/opentelemetry-collector-contrib (Apache-2.0).
LICENSE is unchanged.
