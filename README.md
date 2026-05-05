# Healthcare Data Space

This project extends the **Minimum Viable Dataspace (MVD)** by implementing a realistic healthcare data transaction scenario using the **Eclipse Dataspace Components (EDC)**. It demonstrates secure, sovereign data sharing between two distinct data providers and a consumer.

## Scenario Overview

- **Data Providers**  
  - **Hospital** – Provides anonymized electronic health records (EHR), and patient records and drugs prescribed.  
  - **Pharmaceutical Company** – Provides drug information.  

- **Data Consumer**  
  - **Research Institute** – Requests and integrates datasets from both providers to perform cross-correlation analysis (e.g., drug effectiveness on real-world hospital populations).

## Key Features

- **Eclipse Dataspace Components (EDC)** – Used for all core dataspace functions: identity, contract negotiation, policy enforcement, and data transfer.
- **Extension of MVD** – Builds on the MVD reference implementation, adding assets, policies (e.g., `Access = "research purpose"`), and some new connector.
- **Secure Data Transfer** – Datasets are never exposed via public APIs; all transfers follow usage control policies defined by each provider.
- **Standalone Demo** – Run entirely on Docker.
