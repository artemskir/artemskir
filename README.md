# Artem

**Backend engineer. I ship production systems.**

I build production-ready platforms with business-oriented architectures – from websites and backend services to microservices and LLM-powered solutions. I also ship desktop software for Windows, Linux, and macOS. Open to full-time, contract, and project work worldwide.

[artemskir.com](https://artemskir.com) · [X](https://x.com/artemskir) · [LinkedIn](https://www.linkedin.com/in/artemskir) · [Telegram](https://t.me/artemskir) · [artemsskir@gmail.com](mailto:artemsskir@gmail.com)

---

## Now

- Starting a **Master’s** and taking the [university journal platform](https://github.com/artemskir/university-journal-system) further – the backend is already used by web and mobile clients in the university test contour.
- Operating **[SRbots](https://srbots.ru)** – a cross-platform desktop product I’ve owned since 2022.
- **Actively looking.** Backend / platform roles. Remote, on-site, or relocate – anywhere.



## Selected work



### [University Journal System](https://github.com/artemskir/university-journal-system) – Go backend for a real university

Electronic journal: attendance, grades, assessment forms, async PDF/Excel reports.

Two independently deployed services behind Nginx. **Edge** validates Keycloak JWTs, enforces roles, and routes. **Domain** owns business logic, PostgreSQL, audit, and background workers. Edge never touches the database. Domain never authenticates.

- **94 API routes**, 4 roles, OpenAPI-first (`oapi-codegen`) and type-safe SQL (`sqlc`)
- Load-tested: **500k+ requests**, **~1000 req/s**, avg **~5 ms**, **p95 ~13 ms** (4 Edge replicas, gzip)
- Observability: Prometheus, Grafana, Loki, Tempo · CI/CD deploys on push to `master`

`Go` `Gin` `PostgreSQL` `Keycloak` `Nginx` `Docker` `Prometheus`

### [SRbots](https://srbots.ru) – cross-platform desktop product

Shipped and operated since 2022. Native GUI on **Windows, Linux, and macOS**. Docs: [how it works](https://srbots.ru/docs/how-it-works/).

Concurrent Minecraft protocol clients for **1.8–1.21**, including BungeeCord / Velocity. I own architecture, releases, and distribution.

- Connection lifecycle: register/auth, auto-reconnect, proxy lists with health checks
- Pathfinding (smart / fast / standard) – fast mode cuts route planning ~50×; standard uses ~250% less RAM
- PVP/PVE, chat and command automation, logging, config import
- Scale is hardware-bound: bot count, render distance, and proxy uniqueness are first-class settings

`Desktop` `Networking` `Concurrency` `Proxies` `Wails` `Windows` `Linux` `macOS`

### [Aerial segmentation](https://github.com/artemskir/segmentation-buildings) – ML inference API

Six-class semantic segmentation on aerial imagery (roads, buildings, vegetation, trees, cars, clutter).

U-Net + ResNet34 (ImageNet). FastAPI inference + Streamlit UI.

- Val: **IoU 71.56%**, F1 **82.73%**, accuracy **87.22%** (buildings 97%, cars 99%)
- ~250–450 ms / image on Tesla T4 · ~180 rpm with 4 workers

`Python` `TensorFlow` `FastAPI` `U-Net`

---



## Stack

**Backend:** Go · Python · Java · PostgreSQL · Redis · Gin · Spring · Django  
**Infra:** Docker · Nginx · GitHub Actions · Prometheus · Grafana · Loki  
**Desktop / web:** Wails · React · Node.js  
**ML:** TensorFlow · FastAPI

## Background

- **2022–2026** – B.S. Information Systems and Technologies
- **2025–2026** – Geoinformatics Development with AI Methods
- **2026** – Mathematical Modelling and Applications (UCI, Cuba)
- **2022–present** – SRbots (owner)
- VK **IT-Diving** finalist · Moscow Mayor’s Contest · DevSecOps 2024

Russian (native) · English (B2)

## Contact

[artemsskir@gmail.com](mailto:artemsskir@gmail.com) · [LinkedIn](https://www.linkedin.com/in/artemskir) · [Telegram](https://t.me/artemskir) · [X](https://x.com/artemskir)  
DM me. I read everything.