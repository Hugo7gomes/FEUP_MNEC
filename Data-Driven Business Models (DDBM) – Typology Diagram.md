# Data-Driven Business Models (DDBM) – Typology Diagram

```mermaid
flowchart LR
    %% Axes
    DS[Key Data Sources]
    KA[Key Activities]

    %% Data Sources
    DS1[Free / Open Data]
    DS2[Customer-Provided Data]
    DS3[Tracked & Self-Generated Data]

    %% Key Activities
    KA1[Aggregation]
    KA2[Analytics]
    KA3[Data Generation]

    %% Types
    A[Type A\nFree Data Collector\nand Aggregator]
    B[Type B\nAnalytics-as-a-Service]
    C[Type C\nData Generation\nand Analysis]
    D[Type D\nFree Data Knowledge\nDiscovery]
    E[Type E\nData Aggregation-\nas-a-Service]
    F[Type F\nMulti-Source Data\nMashup and Analysis]

    %% Relationships: Data Sources
    DS1 --> A
    DS1 --> D
    DS1 --> F
    DS2 --> B
    DS2 --> E
    DS2 --> F
    DS3 --> C

    %% Relationships: Key Activities
    KA1 --> A
    KA1 --> E
    KA1 --> F
    KA2 --> B
    KA2 --> D
    KA2 --> F
    KA3 --> C
