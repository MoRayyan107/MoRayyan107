<div align="center">

```
██████╗  █████╗ ██╗   ██╗██╗   ██╗ █████╗ ███╗   ██╗
██╔══██╗██╔══██╗╚██╗ ██╔╝╚██╗ ██╔╝██╔══██╗████╗  ██║
██████╔╝███████║ ╚████╔╝  ╚████╔╝ ███████║██╔██╗ ██║
██╔══██╗██╔══██║  ╚██╔╝    ╚██╔╝  ██╔══██║██║╚██╗██║
██║  ██║██║  ██║   ██║      ██║   ██║  ██║██║ ╚████║
╚═╝  ╚═╝╚═╝  ╚═╝   ╚═╝      ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═══╝
```

### `Backend Software Engineer` · Java · Spring Boot · Distributed Systems

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mohammad%20Rayyan-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mohammad-rayyan-adhoni)
[![Portfolio](https://img.shields.io/badge/Portfolio-rayyanadhoni.netlify.app-10b981?style=flat-square&logo=netlify&logoColor=white)](https://rayyanadhoni-portfolio.netlify.app/)
[![Email](https://img.shields.io/badge/Email-rayyanadhoni107@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:rayyanadhoni107@gmail.com)
[![MEng](https://img.shields.io/badge/MEng-University%20of%20Strathclyde-003865?style=flat-square&logo=graduation-cap&logoColor=white)](https://www.strath.ac.uk)

</div>

---

## ▎Who I Am

I build backend systems with an emphasis on **correctness, scalability, and architectural clarity**. My work centres on the JVM ecosystem — designing REST APIs, modelling relational data, and structuring service layers that remain maintainable as requirements evolve.

Currently deepening expertise in **cloud-native deployment** (Azure Container Apps, Docker) and **event-driven patterns** (Kafka, Redis) to close the gap between system design and production-grade infrastructure.

> *"First, solve the problem. Then, write the code."* — John Johnson

---

## ▎Technical Stack


| Layer | Technologies |
|:---:|:---|
| **Core** | ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![Spring Data JPA](https://img.shields.io/badge/Spring%20Data%20JPA-6DB33F?style=flat-square&logo=spring&logoColor=white) |
| **Databases** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) |
| **Testing** | ![JUnit5](https://img.shields.io/badge/JUnit%205-25A162?style=flat-square&logo=junit5&logoColor=white) ![Mockito](https://img.shields.io/badge/Mockito-78A641?style=flat-square&logo=java&logoColor=white) |
| **Infrastructure** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) |
| **Secondary** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black) |



---

## ▎Project Case Studies

### 🏦 ScotBank — Concurrent Banking System
> `Java` `OOP` `Multi-threaded Design` `JUnit 5`

**The Challenge:**
Model a banking system that handles concurrent account operations without exposing shared state to race conditions or producing inconsistent balances.

**The Solution:**
Designed an object-oriented account hierarchy with strict encapsulation boundaries. Applied thread-safe patterns to transaction operations, ensuring **atomicity across deposit, withdrawal, and transfer flows**. Separated account state from business logic to enable isolated unit testing of each operation type.

[![ScotBank Repo](https://img.shields.io/badge/View%20Repository-ScotBank-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/MoRayyan107/ScotBank)

---

### 💬 Discord — Real-time Messaging Service
> `Java` `Concurrent I/O` `Event-driven Architecture` `Socket Programming`

**The Challenge:**
Build a distributed, multi-user messaging service capable of handling simultaneous connections across multiple server instances with real-time message propagation.

**The Solution:**
Implemented a server architecture using Java's concurrency primitives — replacing raw thread-per-client with a fixed ExecutorService thread pool, and decoupling message delivery from sending via BlockingQueue with dedicated dispatcher threads. Extended to a distributed system using Kafka for cross-server messaging and Redis for shared group state and user routing.

```
Client (TCP Socket)
        ↓
ClientHandler (Thread Pool — 200 threads)
        ↓
SafeGroupChat (BlockingQueue + dispatcher thread)
        ↓
KafkaProducer → Kafka Cluster → KafkaConsumer
        ↓
Redis (group membership, user-server routing)
        ↓
Target ClientHandler → sendToClient()
```

[![Discord Repo](https://img.shields.io/badge/View%20Repository-Discord%20App-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/MoRayyan107/Discord)

---

## ▎Engineering Roadmap

```
2024 ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 2025+
  │                                                              │
  ├─ [✓] Spring Boot & REST API design                          │
  ├─ [✓] PostgreSQL schema design & JPA modelling               │
  ├─ [✓] JUnit 5 + Mockito test coverage                        │
  ├─ [✓] Docker containerisation                                │
  ├─ [✓] Azure Container Apps deployment                        │
  │                                                              │
  ├─ [ ] Apache Kafka — event streaming pipelines               │
  ├─ [ ] Redis — distributed caching layer                      │
  ├─ [ ] GitHub Actions — full CI/CD pipelines                  │
  └─ [ ] Distributed tracing & observability                    │
```

---

## ▎Certifications

| Certificate | Issuer | Focus |
|:---|:---|:---|
| 🏆 JPMC Forage Job Simulation | JPMorgan Chase & Co. | Software Engineering |

---

<div align="center">

**Open to backend engineering roles, internships, and collaborations.**

`rayyanadhoni107@gmail.com` · [LinkedIn](https://www.linkedin.com/in/mohammad-rayyan-adhoni) · [Portfolio](https://rayyanadhoni-portfolio.netlify.app/)

</div>
