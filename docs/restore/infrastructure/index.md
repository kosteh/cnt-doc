---
layout: default
parent: Restore
title: Infrastructure
nav_order: 100
has_children: false
---

# Infrastructure

## Introduction
The infrastructure to support *restore tests* is named the **Restore Test Omgeving (RTO)**. This environment is/will be made available at the **PLP platform** (named **PLP-RTO**) and the **Azure PLS platform** (named **PLS-RTO**). 

```mermaid
flowchart TD
    direction LR
    subgraph PLP["PLP (on-premise)"]
        subgraph PLP-ONT["ONT\nenvironment"]
        end
        subgraph PLP-INT["INT\nenvironment"]
        end
        subgraph PLP-FTO["FTO\nenvironment"]
        end
        subgraph PLP-RTO["RTO\nenvironment"]
        end
        subgraph PLP-PROD["PROD\nenvironment"]
        end
    end
    
    subgraph PLS["PLS (Azure)"]
        subgraph AZ-TEST["TEST\nsubscriptions"]
        end
        subgraph AZ-RTO["RTO\nsubscriptions"]
        end
        subgraph AZ-PROD["PROD\nsubscriptions"]
        end
    end

    classDef BLUE fill:#109AEB
    classDef BLUE-DASH fill:#109AEB,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 2 2

    PLP-ONT <--> AZ-TEST
    PLP-INT <--> AZ-TEST
    PLP-FTO <--> AZ-TEST
    PLP-RTO:::BLUE <-.->|RTO network| AZ-RTO:::BLUE-DASH
    PLP-PROD <--> AZ-PROD
```

The current status of the RTO environment is:
- The PLP-RTO environment is functionally available and usable. *Access to this new environment must, however, be requested.*
- The PLS-RTO enviroment is currently in the design phase. The PLS platform will be upgraded in the coming months to support this new environment. 
- The RTO network connection between PLP-RTO and PLS-RTO is also in the design phase.

