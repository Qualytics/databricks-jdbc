# NEXT CHANGELOG

## [Unreleased]

### Added
- Enabled direct results by default in SEA mode to improve latency for short and small queries.
### Updated
- Telemetry data is now captured more efficiently and consistently due to enhancements in the log and connection close flush logic.
- Updated Databricks SDK version to v0.65.0 (This is to fix OAuthClient to properly encode complex query parameters.)
- Added IgnoreTransactions connection parameter to silently ignore transaction method calls.

### Fixed
- Fixed state leaking issue in thrift client.
- Fixed timestamp values returning only milliseconds instead of the full nanosecond precision.
- Fixed complex data type conversion issues by improving StringConverter to handle Databricks complex objects (arrays/maps/structs), JDBC arrays/structs, and generic collections.
- Fixed ComplexDataTypeParser to correctly parse ISO timestamps with T separators and timezone offsets, preventing Arrow ingestion failures.
- Fixed Statement.getUpdateCount() for DML queries.
- Fixed Maven Central publishing to use minimal POM for both main and thin JARs, restoring behavior from v1.0.7 and earlier
---
*Note: When making changes, please add your change under the appropriate section with a brief description.* 
