# NEXT CHANGELOG

## [Unreleased]

### Added

### Updated

### Fixed
- Fixed timestamp values returning only milliseconds instead of the full nanosecond precision.
- Fixed complex data type conversion issues by improving StringConverter to handle Databricks complex objects (arrays/maps/structs), JDBC arrays/structs, and generic collections.
- Fixed ComplexDataTypeParser to correctly parse ISO timestamps with T separators and timezone offsets, preventing Arrow ingestion failures.
---
*Note: When making changes, please add your change under the appropriate section with a brief description.* 
