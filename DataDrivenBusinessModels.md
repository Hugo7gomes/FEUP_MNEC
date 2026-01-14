# Data-Driven Business Models (DDBM) – Comparison Table

| DDBM Type | Key Data Sources | Key Activities | Value Proposition | Target Customers | Revenue Model |
|----------|-----------------|----------------|------------------|------------------|---------------|
| **Type A – Free Data Collector and Aggregator** | Mostly free and open data, social media data, crowdsourced data, some proprietary acquired data | Data collection, aggregation, limited crawling, basic visualization, data distribution (e.g., via APIs) | Easy and reliable access to multiple heterogeneous data sources through a single interface | B2B and B2C | Advertising, brokerage fees, subscription fees, usage fees |
| **Type B – Analytics-as-a-Service** | Customer-provided data combined with external datasets | Data collection, analytics, visualization, API-based delivery of insights | Actionable insights and knowledge derived from analytics on customer data (e.g., marketing, fraud detection, customer behavior) | B2B | Subscription fees, usage-based fees |
| **Type C – Data Generation and Analysis** | Self-generated data (tracked, generated, crowdsourced) | Data generation, tracking, aggregation, analytics | Combined data and analytics outputs (e.g., web analytics, leads, performance metrics) | B2B | Usage-based fees, asset sales (e.g., devices, sensors) |
| **Type D – Free Data Knowledge Discovery** | Free and publicly available data (social media, review sites, Q&A platforms, financial and web data) | Web crawling, data aggregation, analytics | Identification and prediction of trends, influencers, and patterns in real time | B2B and B2C | Subscription fees, usage-based fees, advertising, brokerage fees |
| **Type E – Data Aggregation-as-a-Service** | Customer-owned internal data | Data aggregation, organization, visualization, data distribution through interfaces | Structured and unified view of fragmented customer data, simplifying data management | B2B, B2B2C | Subscription fees, usage-based fees |
| **Type F – Multi-Source Data Mashup and Analysis** | Combination of customer-provided data and free/external data (web-scraped) | Data aggregation, data enrichment, analytics, data generation (web scraping) | Enriched and benchmarked analytics by combining internal and external data sources | Mostly B2B | Subscription-based models |



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

