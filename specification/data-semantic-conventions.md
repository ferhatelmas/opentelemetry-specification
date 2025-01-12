# Semantic Conventions

These documents define standard names and values of Resource labels and
Span attributes.

* [Resource Conventions](data-resource-semantic-conventions.md)
* [Span Conventions](#span-conventions)

## Span Conventions

In OpenTelemetry spans can be created freely and it’s up to the implementor to
annotate them with attributes specific to the represented operation. Spans
represent specific operations in and between systems. Some of these operations
represent calls that use well-known protocols like HTTP or database calls.
Depending on the protocol and the type of operation, additional information
is needed to represent and analyze a span correctly in monitoring systems. It is
also important to unify how this attribution is made in different languages.
This way, the operator will not need to learn specifics of a language and
telemetry collected from multi-language micro-service can still be easily
correlated and cross-analyzed.

The following semantic conventions for spans are defined:

* [HTTP](data-http.md): Spans for HTTP client and server.
* [Database](data-database.md): Spans for SQL and NoSQL client calls.
* [RPC/RMI](data-rpc.md): Spans for remote procedure calls (e.g., gRPC).
