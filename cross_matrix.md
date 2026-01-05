```mermaid
flowchart LR
    subgraph TIE["Tenable Identity Exposure (Alsid)"]
        T1["Audience: Executives / Auditors"]
        T2["Access Model: Admin-only UI"]
        T3["Data Access: Limited export (CSV focus)"]
        T4["Visualization: Pre-built widgets (static)"]
        T5["Analysis Depth: Opinionated risk summaries"]
        T6["Operational Use: Low outside admin team"]
        T7["Marketing Positioning: Identity Risk Platform"]
    end

    subgraph BH["BloodHound (Enterprise Edition)"]
        B1["Audience: Security Engineers / Red Teams"]
        B2["Access Model: Broad RBAC / Read-only views"]
        B3["Data Access: Full graph + API access"]
        B4["Visualization: Interactive attack graphs"]
        B5["Analysis Depth: Ground-truth attack paths"]
        B6["Operational Use: High across security org"]
        B7["Positioning: Active Directory Attack Path Analysis"]
    end

    T1 --- B1
    T2 --- B2
    T3 --- B3
    T4 --- B4
    T5 --- B5
    T6 --- B6
    T7 --- B7
