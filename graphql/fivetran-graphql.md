# Fivetran GraphQL Schema

Conceptual GraphQL schema for the Fivetran managed data pipeline service. Fivetran provides automated data integration with 500+ pre-built connectors that sync data from SaaS applications, databases, and APIs into cloud data warehouses.

## Source

Derived from the Fivetran REST API documentation:
- https://fivetran.com/docs/rest-api
- https://fivetran.com/docs/rest-api/getting-started
- https://github.com/fivetran

## Coverage

The schema covers the following resource domains:

- **Users and Access**: User, Role, Membership, TeamMembership
- **Groups and Teams**: Group, Team
- **Connectors**: Connector, ConnectorConfig, ConnectorSchema, ConnectorType, ConnectorAuth, ConnectorStatus, GroupConnector
- **Destinations**: Destination, DestinationConfig, DestinationType
- **Schemas and Metadata**: Schema, Table, Column, SchemaReloadStatus, MetadataConnector, MetadataTable, MetadataColumn, Privacy, PrivacyMask
- **Transformations**: DbtTransformation, DbtProject, DbtModel
- **Syncs**: Sync, SyncStatus, HistoricalSync, Pause, Trigger, Schedule
- **Webhooks**: Webhook
- **Usage and Billing**: Usage, UsageSummary, DailyActiveRows, Limit, Dashboard
- **Security**: Certificate, FingerPrint, ApiConfig
- **Setup and Configuration**: Setup, Metadata

## Types Count

55 types defined in `fivetran-schema.graphql`.
