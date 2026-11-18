### Hi, I'm Ömer

Full-stack developer in Istanbul. Most of my work is Java 21 / Spring Boot on the backend and React on the front, usually around data that arrives messy from several places and has to end up clean, queryable and on a chart.

At work I've been building things like:

- a sea-level monitoring service that pulls from five outside sources (REST, CSV, FTP, one custom binary format), stores it in PostgreSQL and serves it fast enough to chart years of data
- a matching pipeline where rules go first, a local LLM (Qwen on Ollama) only gets the cases the rules can't decide, and anything still uncertain goes to a person whose answer the system remembers next time
- the admin console and access management for an ISO 27001 compliant SSO system, plus the integration work around its OAuth2 gateway

That code belongs to my employer, so the repos below are my own rewrites of the same ideas, written from scratch with made-up data.

**Backend / data**

- [monitoring-hub](https://github.com/Omercanbasboga/monitoring-hub) · one API over four very different sensor feeds (Spring Boot, Spring Batch, PostgreSQL)
- [minmax-lttb-downsampler](https://github.com/Omercanbasboga/minmax-lttb-downsampler) · shrink 30k points to 300 without losing the spike you actually care about
- [sso-gateway-bff](https://github.com/Omercanbasboga/sso-gateway-bff) · reactive OAuth2/OIDC backend-for-frontend (Spring Cloud Gateway)
- [installment-scheduler](https://github.com/Omercanbasboga/installment-scheduler) · BNPL style payment plans, mostly about not losing a cent to rounding
- [tallyup](https://github.com/Omercanbasboga/tallyup) · group expenses settled with as few transfers as possible

**Frontend**

- [monitoring-hub-dashboard](https://github.com/Omercanbasboga/monitoring-hub-dashboard) · React charts for the service above
- [iam-admin-console](https://github.com/Omercanbasboga/iam-admin-console) · clients, users, roles and scopes for the gateway
- [org-management-console](https://github.com/Omercanbasboga/org-management-console) · members, meetings, budget and an approval queue

**Games, for fun**

- [hollowmere](https://omercanbasboga.github.io/hollowmere/) · match-3 where you seal monsters, with a small [live-ops config service](https://github.com/Omercanbasboga/hollowmere-liveops)
- [hollowmere-vigil](https://omercanbasboga.github.io/hollowmere-vigil/) · short branching text adventure in the same world

Java · Spring Boot · Spring Batch · PostgreSQL · Redis · React · Node.js · Docker · Ollama

[Website](https://omercanbasboga.github.io) · [LinkedIn](https://www.linkedin.com/in/%C3%B6mer-can-ba%C5%9Fbo%C4%9Fa-b7940223a)
