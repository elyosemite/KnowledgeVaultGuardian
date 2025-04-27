# Project Structure

```mermaid
graph TD
    A[Knowledge Base] --> B[Core Technologies]
    A --> C[Cross-Cutting Concerns]
    A --> D[Architecture & Patterns]
    A --> E[Learning Paths]
    A --> F[News & Updates]
    
    B --> B1[Languages]
    B1 --> B1a[C#/.NET]
    B1 --> B1b[TypeScript]
    B1 --> B1c[Haskell]
    
    B --> B2[Platforms]
    B2 --> B2a[Docker]
    B2 --> B2b[Kubernetes]
    
    C --> C1[Networking]
    C1 --> C1a[HTTP/HTTPS]
    C1 --> C1b[TCP/IP]
    C1 --> C1c[Async Messaging]
    
    C --> C2[Security]
    C2 --> C2a[Cryptography]
    C2 --> C2b[OWASP]
    
    D --> D1[Design Patterns]
    D1 --> D1a[Creational]
    D1 --> D1b[Structural]
    D1 --> D1c[Behavioral]
    
    D --> D2[Arch Styles]
    D2 --> D2a[Microservices]
    D2 --> D2b[Event-Driven]
    D2 --> D2c[Serverless]
    
    E --> E1[Certifications]
    E --> E2[Roadmaps]
    
    F --> F1[Release Notes]
    F --> F2[RFC Analysis]
```

## Detailed Folder Structure

```bash
/knowledge-base
│
├── core-technologies/
│   ├── languages/
│   │   ├── csharp/
│   │   │   ├── frameworks/
│   │   │   │   ├── aspnet-core.md
│   │   │   │   └── entity-framework.md
│   │   │   ├── performance/
│   │   │   ├── memory-management.md
│   │   │   └── language-features.md
│   │   │
│   │   ├── haskell/
│   │   │   ├── functional-patterns.md
│   │   │   └── concurrency.md
│   │   │
│   │   └── typescript/
│   │       ├── type-system.md
│   │       └── framework-integrations.md
│   │
│   └── platforms/
│       ├── docker/
│       │   ├── compose.md
│       │   └── security.md
│       │
│       └── kubernetes/
│           ├── networking.md
│           └── operators.md
│
├── architecture-patterns/
│   ├── design-patterns/
│   │   ├── creational/
│   │   │   └── factory-patterns.md
│   │   ├── structural/
│   │   └── behavioral/
│   │
│   └── architecture-styles/
│       ├── microservices/
│       │   ├── decomposition.md
│       │   └── interservice-comm.md
│       │
│       └── event-driven/
│           ├── event-sourcing.md
│           └── cqrs.md
│
├── infra-networking/
│   ├── protocols/
│   │   ├── http-versions.md
│   │   └── tcp-ip-stack.md
│   │
│   └── messaging-systems/
│       ├── rabbitmq/
│       └── kafka/
│
├── learning-resources/
│   ├── certifications/
│   │   ├── az-204.md
│   │   └── cka.md
│   │
│   └── roadmaps/
│       ├── backend-2024.md
│       └── devops.md
│
├── news-updates/
│   ├── dotnet-releases.md
│   └── kubernetes-changelogs.md
│
└── _global/
    ├── glossary.md
    ├── cross-references.md
    └── ARCHIVE.md
```

## Categorization System

### Technology Matrix

| Dimension        | Tags Example                          |
|------------------|---------------------------------------|
| **Stack Layer**      | #Frontend, #Backend, #Infrastructure  |
| **Complexity Level** | #101, #201, #301, #401                |
| **Content Type**     | #Tutorial, #DeepDive, #CheatSheet     |

### File Naming Convention
[Technology]_[Topic]_[Version].md

Example:  
- csharp_linq-optimization_net8.md  
- kubernetes_network-policies_v1.28.md
