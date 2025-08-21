Diagrams

Material for MkDocs allows you to easily implement statically rendered diagrams in your documentation. Examples of diagrams you might include are:

    Flow charts
    Sequence diagrams
    State diagrams
    Class diagrams
    Entity-relationship diagrams


## Flowcharts
```mermaid
graph LR
  A[Start] --> B{Failure?};
  B -->|Yes| C[Investigate...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Success!];
```

## Sequence Diagrams

```mermaid
sequenceDiagram
  autonumber
  Server->>Terminal: Send request
  loop Health
      Terminal->>Terminal: Check for health
  end
  Note right of Terminal: System online
  Terminal-->>Server: Everything is OK
  Terminal->>Database: Request customer data
  Database-->>Terminal: Customer data
```