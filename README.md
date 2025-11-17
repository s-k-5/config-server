# Config Server – Hotel Review System
This repository stores the **centralized configuration files** for the [Hotel Review System](https://github.com/s-k-5/hotel-review-system).

---

## Structure:
```
config-repo/
├── auth-service.yml
├── user-service.yml
├── hotel-service.yml
├── review-service.yml
├── api-gateway.yml
└── eureka-service.yml

```

---

## How it Works
- Runs on **port 8888**.
- Backed by **Spring Cloud Config Server**.
- Each microservice loads its configuration based on `spring.application.name`.  
- Example: `user-service` → `user-service.yml`.

## Benefits
- Centralized management of DB, JPA, Eureka, and logging configs.
- Easy environment promotion (dev → staging → prod) via Git branches.
- Supports encrypted secrets or Vault integration in future.

---
