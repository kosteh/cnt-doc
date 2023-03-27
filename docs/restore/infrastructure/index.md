---
layout: default
parent: Restore
title: Infrastructure
nav_order: 100
has_children: true
---

# Infrastructure

## Introduction
The infrastructure to support *restore tests* is named the **Restore Test Omgeving (RTO)**. This environment is available at the **PLP platform (named PLP-RTO)** as well as at the **Azure PLS platform (named PLS-RTO)**.

```mermaid
flowchart TD
    direction LR
    subgraph PLP
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
    subgraph AZURE
        subgraph AZ-TEST["TEST\nsubscriptions"]
        end
        subgraph AZ-RTO["RTO\nsubscriptions"]
        end
        subgraph AZ-PROD["PROD\nsubscriptions"]
        end
    end

    classDef BLUE fill:#109AEB
    PLP-ONT <--> AZ-TEST
    PLP-INT <--> AZ-TEST
    PLP-FTO <--> AZ-TEST
    PLP-RTO:::BLUE <--> AZ-RTO:::BLUE
    PLP-PROD <--> AZ-PROD
```

## Requesting access to the PLP-RTO
Unlike the normal PLP selfservice  
