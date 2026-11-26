# Hi, I'm Abdulhadi Almohammad 👋

**Front-end Developer & UI/UX Designer**: React · TypeScript · Figma
📍 Syria · 🗣 Arabic · English

I design products in Figma, then build them myself in React and TypeScript, so the design ships as drawn: responsive, fast and accessible. Arabic-first and RTL by default, with real loading, empty and error states, and a service layer that switches from a mock server to a real backend with a single variable.

🌐 [**Portfolio: abdulhadi.review**](https://abdulhadi.review) · ✉️ [aboshkar38@gmail.com](mailto:aboshkar38@gmail.com) · 💬 [Telegram](https://t.me/Abood_352) · 📱 [WhatsApp](https://wa.me/963996710002) · 📷 [Instagram](https://www.instagram.com/engineer_352)

## 🛠 Tech Stack

![React](https://img.shields.io/badge/React_19-20232A?style=flat&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat&logo=angular&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white)
![CSS](https://img.shields.io/badge/CSS_Modules-1572B6?style=flat&logo=css3&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat&logo=threedotjs&logoColor=white)
![GSAP](https://img.shields.io/badge/GSAP-88CE02?style=flat&logo=greensock&logoColor=black)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat&logo=figma&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)

**UX:** UX research · prototyping · design systems (shared tokens and components between Figma and code) · accessibility (keyboard and screen-reader support)
**Front-end architecture:** one typed service layer per app · in-browser mock server · hash routing · i18n (Arabic / English) · light and dark themes · build-time prerendering
**Arabic-first:** RTL layouts · Arabic search that ignores hamza and taa marbuta · Hijri dates · Saudi payment flows (mada, Apple Pay, BNPL)

## 💼 Live Apps (2026)

Eight standalone products, each with a customer side and a business dashboard. All open in the browser with seeded demo data, no sign-up needed.

| Project | Domain | Highlights |
|---|---|---|
| [Raff · رفّ](https://abdulhadi.review/projects/raff/) · [code](https://github.com/abood352/raff) | E-commerce | Saudi handcrafts store: Arabic search, server-priced cart with 15% VAT and promo codes, mada / 3-D Secure / Apple Pay / BNPL checkout, merchant dashboard with stock and CSV export |
| [Sada · صدى](https://abdulhadi.review/projects/sada/) · [code](https://github.com/abood352/sada) | Event ticketing | Two-level seat map with family sections, 8-minute holds, virtual queue, QR tickets that refresh every 30 s, transfers and refunds, organizer gate scanner |
| [Sufra · سفرة](https://abdulhadi.review/projects/sufra/) · [code](https://github.com/abood352/sufra) | Food delivery | Order from nearby restaurants, follow the courier live on the map; restaurant dashboard receives orders in real time |
| [Dar · دار](https://abdulhadi.review/projects/dar/) · [code](https://github.com/abood352/dar) | Real estate | Map search, price vs. neighbourhood, mortgage calculator, viewing bookings and an agent dashboard |
| [Midad · مِداد](https://abdulhadi.review/projects/midad/) · [code](https://github.com/abood352/midad) | AI writing | Arabic writing assistant: streamed chat, ready templates, tone control and a documents editor |
| [Qist · قسط](https://abdulhadi.review/projects/qist/) · [code](https://github.com/abood352/qist) | Fintech / BNPL | Buy now, pay later in 4 interest-free instalments, limits and due dates in one place, merchant dashboard |
| [Mawid · موعد](https://abdulhadi.review/projects/mawid/) · [code](https://github.com/abood352/mawid) | Healthcare | Find a doctor, book for yourself or family, follow your queue after check-in, reception dashboard |
| [Nuzul · نُزُل](https://abdulhadi.review/projects/nuzul/) · [code](https://github.com/abood352/nuzul) | Hospitality | Chalet and rest-house booking with nightly pricing on the calendar, self check-in codes, host dashboard |

### ⭐ Raff (رفّ): E-commerce Store & Merchant Dashboard · Design + Front-end
[Live](https://abdulhadi.review/projects/raff/) · [code](https://github.com/abood352/raff)

**The idea.** Small craft brands sell through social-media messages: one photo, a "how much?", then a long chat to confirm colour, address and payment, and the buyer never sees the final price with VAT and shipping until the end. Raff shows every colour with its own image and VAT-inclusive price, prices the cart on the "server" before payment, and keeps checkout to three short steps with the payment methods Saudi shoppers actually use.

| Area | What I built |
|---|---|
| 🔎 **Discovery** | Arabic search that ignores hamza and taa marbuta, instant suggestions, filters by craft, price, colour and stock that live in the URL |
| 🛒 **Cart & pricing** | Server-side repricing: 15% VAT, free shipping over SAR 300, promo codes |
| 💳 **Checkout** | mada and cards with 3-D Secure, Apple Pay, instalments and cash on delivery; national address, Saudi mobile and Hijri date on the order |
| 📊 **Merchant dashboard** | Sales, stock, promo codes, customers and CSV export |

- **Front-end:** React 19 · TypeScript · Vite · hash routing · build-time prerender of the first screen · Arabic / English · light / dark · mobile-first.
- **Architecture:** one service layer (`api/services.ts`) backed by an in-browser mock server with business rules; a real-API build ships none of the mock code. API contract, database schema and architecture are documented in `docs/`.

### ⭐ Sada (صدى): Event Ticketing with a Seat Map · Design + Front-end
[Live](https://abdulhadi.review/projects/sada/) · [code](https://github.com/abood352/sada)

**The idea.** On-sale moments are chaos: two people grab the same seat, screenshots of tickets leak, families don't know where to sit, and gates can't tell a valid ticket from a used one. Sada holds seats while you pay, names every ticket and rotates its QR code, and gives organizers a live view and a gate scanner.

| Area | What I built |
|---|---|
| 🎟 **Seat map** | Two-level SVG venue map with pan and zoom, price colours, family sections, best-available picker, and a list picker for keyboard and screen-reader users |
| ⏱ **Holds & queue** | 8-minute seat holds, orphan-seat rules, wheelchair spaces booked with a companion seat, virtual queue for hot events |
| 📱 **Tickets** | Named tickets with a QR that changes every 30 seconds, transfer to a phone number, refunds up to 48 hours before the event |
| 🏟 **Organizer** | Sales and revenue, pause/resume sales, live check-in seat map, gate scanner that reports used, refunded, expired and wrong-gate tickets |

- **Front-end:** React 19 · TypeScript · CSS Modules · SVG seat rendering with event delegation · phone OTP sign-in · Arabic / English · light / dark.
- **Domain logic:** fee and VAT pricing, promo rules, per-order and per-person limits, and refund policy, all shared between the UI and the mock server.

## 🎨 Product Design & Interactive Prototypes (2024–2025)

Designed in Figma and built as working, clickable prototypes in React and TypeScript.

| Project | Domain | Highlights |
|---|---|---|
| [Jamiaty · جامعتي](https://github.com/abood352/jamiaty) | University management | Course registration with instant schedule-conflict and prerequisite checks, sections and rooms, grades by role, fees and receipts, student portal |
| [Sarraf · صرّاف](https://github.com/abood352/sarraf) | Digital wallet | Multi-currency wallet: instant transfers, bill payments and a monthly budget |
| [Masar · مسار](https://github.com/abood352/masar) | Fleet tracking | Live map of delivery vehicles with delay and stop alerts |
| [Nabd · نبض](https://github.com/abood352/nabd) | SaaS marketing | Product site for an uptime monitoring and status-pages service |
| [Kawader · كوادر](https://github.com/abood352/kawader) | HR | Employee records, attendance, leave and payroll in one dashboard |
| [Manhal · منهل](https://github.com/abood352/manhal) | E-learning | Arabic programming courses: short lessons, exercises and a completion certificate |

## 🧭 The Portfolio Itself

[**abood352/portfolio**](https://github.com/abood352/portfolio): an interactive 3D gallery room you walk through by scrolling, with six view modes, light and dark themes with real scene lighting, a mini star-hunt game, and an automatic simple HTML mode when WebGL isn't available. React · Three.js (React Three Fiber / drei) · GSAP ScrollTrigger · Lenis.

## 🤝 How I Work

- **Design and code by the same hands:** tokens and components carry over from Figma to React, so nothing gets lost in handoff.
- **Real states:** loading, empty and error screens are designed, not left to chance.
- **Accessible by default:** keyboard navigation, screen-reader labels and checked contrast.
- **Backend-ready:** every app talks to one typed service layer with a documented API contract, so connecting a real backend is a config change.

📫 Open to freelance projects and full-time front-end / UI-UX roles.
