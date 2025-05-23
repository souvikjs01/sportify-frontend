# 🎧 Spotify – Spotify-Inspired Music Application.

It is a full-featured, Spotify-inspired music streaming application built using a **microservice architecture**. It includes two backend services (`user-service` and `admin-service`) and a modern React frontend. The system uses **Redis** caching for high performance and faster response times.

---

## 🧱 Architecture Overview

                 ┌─────────────┐
                 │   Frontend  │ (React.js + TailwindCSS)
                 └──────┬──────┘
                        │
         ┌──────────────┴──────────────┐
         │                             │
 ┌───────▼────────┐           ┌────────▼────────┐
 │  user-service  │           │ admin-service   │
 │ (Music, Auth)  │           │ (Manage Songs)  │
 └───────┬────────┘           └────────┬────────┘
         │                             │
      ┌──▼────┐                   ┌─────▼───┐
      │ Redis │ ◀──────────────▶ │Pg, Mongo│
      └───────┘                   └──────────┘

