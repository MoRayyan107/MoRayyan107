<div align="center">

```
██████╗  █████╗ ██╗   ██╗██╗   ██╗ █████╗ ███╗   ██╗
██╔══██╗██╔══██╗╚██╗ ██╔╝╚██╗ ██╔╝██╔══██╗████╗  ██║
██████╔╝███████║ ╚████╔╝  ╚████╔╝ ███████║██╔██╗ ██║
██╔══██╗██╔══██║  ╚██╔╝    ╚██╔╝  ██╔══██║██║╚██╗██║
██║  ██║██║  ██║   ██║      ██║   ██║  ██║██║ ╚████║
╚═╝  ╚═╝╚═╝  ╚═╝   ╚═╝      ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═══╝
```

### `Backend Software Engineer` · Java · Spring Boot 

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mohammad%20Rayyan-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mohammad-rayyan-adhoni)
[![Portfolio](https://img.shields.io/badge/Portfolio-rayyanadhoni.netlify.app-10b981?style=flat-square&logo=netlify&logoColor=white)](https://rayyanadhoni-portfolio.netlify.app/)
[![Email](https://img.shields.io/badge/Email-rayyanadhoni107@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:rayyanadhoni107@gmail.com)
[![MEng](https://img.shields.io/badge/MEng-University%20of%20Strathclyde-003865?style=flat-square&logo=graduation-cap&logoColor=white)](https://www.strath.ac.uk)

</div>

---

## ▎Who I Am
### Hi there 👋🏼, I'm Rayyan Adhoni

**Backend Software Engineer | Java • Spring Boot**

I build backend systems with an emphasis on **correctness, scalability, and architectural clarity**. My work centres on the JVM ecosystem — designing REST APIs, modelling relational data, and struct[...]

Currently deepening expertise in **cloud-native deployment** (Azure Container Apps, Docker) and **event-driven patterns** (Kafka, Redis) to close the gap between system design and production-grade inf[...]

> *"First, solve the problem. Then, write the code."* — John Johnson

---

## ▎Technical Stack


| Layer | Technologies |
|:---:|:---|
| **Core** | ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=sp[...]
| **Databases** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&l[...]
| **Testing** | ![JUnit5](https://img.shields.io/badge/JUnit%205-25A162?style=flat-square&logo=junit5&logoColor=white) ![Mockito](https://img.shields.io/badge/Mockito-78A641?style=flat-square&logo=jav[...]
| **Infrastructure** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=mic[...]
| **Secondary** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&log[...]



---

## ▎Project Case Studies

### 🏦 ScotBank — Concurrent Banking System
> `Java` `OOP` `Jooby` `JUnit 5` `Mockito`

**The Task:**
Develop a foundational banking application architecture, emphasizing strict encapsulation and clear separation between business logic and account state to ensure maintainable, testable code with cover[...]

**The Solution:**
Using the Jooby framework, an object-oriented account hierarchy with stringent encapsulation boundaries was designed. For isolated unit testing, service-oriented endpoints for deposit, withdrawal, and[...]

[![ScotBank Repo](https://img.shields.io/badge/View%20Repository-ScotBank-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/MoRayyan107/ScotBank)

---

### 💬 Discord — Real-time Messaging Service 
> `Java` `Concurrent I/O` `Event-driven Architecture` `Socket Programming`

**The Challenge:**
Build a distributed, multi-user messaging service capable of handling simultaneous connections across multiple server instances with real-time message propagation.

**The Solution:**
Implemented a server architecture using Java's concurrency primitives — replacing raw thread-per-client with a fixed ExecutorService thread pool, and decoupling message delivery from sending via Blo[...]

```
Client (TCP Socket)
        ↓
ClientHandler (Thread Pool — 200 threads)
        ↓
SafeGroupChat (BlockingQueue + dispatcher thread)
        ↓
KafkaProducer → KafkaConsumer (For Cross-server Messaging)
        ↓
Redis (group membership, user-server routing)
        ↓
Target ClientHandler → sendToClient()
```

[![Discord Repo](https://img.shields.io/badge/View%20Repository-Discord%20App-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/MoRayyan107/Discord)

---

### 🚨 ValutGuard — Real-time Fraud Detecting Ssytem
> `Java 21` `Spring Boot` `Apache Kafka` `Redis` `PostgreSQL` `Spring Security` `WebSocket`

**The Main Objetive:**

Every day, globally  many finance banks handels million and billions of transactions, and in this era fraud is getting more and more complex. So, I'm developing a fraud detecting engine that runs with[...]
This engine validates, ingets incomming transactions and calculate risk scoring in real-time via web-sockets. processing transactions and calculatig risk score in parallel is the main challenge here

**The Solution:**

!!ON WORK

key idea on flow:
```
External Service / Payment Gateway
        ↓
Filter Chain (CORS → JWT Auth → Redis Rate Limiter)
        ↓
Controller → Service Layer (Validation)
        ↓                        ↓
Save to PostgreSQL       Kafka Producer → to a Topic
        ↓                        ↓
Return 200 OK          Kafka Consumer (Fraud Scoring Engine)
                                 ↓                    ↓
                        Score >= 0.7 → FLAGGED    Score < 0.7 → COMPLETED
                                 ↓
                        Persist to DB + WebSocket Alert  
                                        
```



[![VaultGuard Repo](https://img.shields.io/badge/View%20Repository-VaultGuard-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/MoRayyan107/VaultGuard)


---


## ▎Engineering Roadmap

```
2024 ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━[...]
 │                                                                           │
 ├─ [✓] Spring Boot & REST API design                                        │
 ├─ [✓] PostgreSQL schema design & JPA modelling                             │
 ├─ [✓] JUnit 5 + Mockito test coverage                                      │
 ├─ [✓] Docker containerisation                                              │
 ├─ [✓] Azure Container Apps deployment                                      │
 │                                                                           │
 ├─ [ ] Distributed Caching (Redis) — TTLs, Eviction Policies, Cache-Aside   │
 ├─ [ ] Event-Driven Architecture (Kafka) — Topics, Partitions, Consumers    │
 ├─ [ ] Advanced CI/CD (GitHub Actions) — Automated testing & Deployment     │
 ├─ [ ] Observability (ELK/Grafana) — Log aggregation & Custom Metrics       │
 ├─ [ ] Distributed Tracing — OpenTelemetry & Jaeger                         │
 └─ [ ] Infrastructure as Code (Terraform) — Automated Azure provisioning    │
```

---

## ▎Certifications

| Certificate | Issuer | Focus |
|:---|:---|:---|
| JPMC Forage Job Simulation | JPMorgan Chase & Co. | Software Engineering |

---

## ▎GitHub Activity

[![Rayyan's github activity graph](https://github-readme-activity-graph.vercel.app/graph?username=MoRayyan107&bg_color=1a1b27&color=ce9ffc&line=636e72&point=ff7b72&area=true&hide_border=true)](https://github.com/ashutosh00710/github-readme-activity-graph)

[![GitHub Streak](https://streak-stats.demolab.com?user=MoRayyan107&theme=dark)](https://git.io/streak-stats)

---

<div align="center">

**Open to backend engineering roles, internships, and collaborations.**

`rayyanadhoni107@gmail.com` · [LinkedIn](https://www.linkedin.com/in/mohammad-rayyan-adhoni) · [Portfolio](https://rayyanadhoni-portfolio.netlify.app/)

</div>
