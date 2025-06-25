# Clínica Roriz Linhares – No-Show Reduction SPA

[Live Demo](https://rodrigomarquest.github.io/rorizlinhares/) · [Project Board](https://github.com/users/rodrigomarquest/projects/1/views/1)

## About

This Single-Page Application (SPA) is the prototype submitted for the **Customer Engagement & AI** module of the MSc in Artificial Intelligence for Business (Technological University Dublin). Its goal is to minimise appointment *no-shows* and early drop-off rates at **Clínica Roriz Linhares** in Goiânia, Brazil, by streamlining booking, automating reminders and maintaining patient engagement between sessions.

## Features

* 📅 **Self-service booking wizard** with real-time slot validation
* 🔔 **Automated multi-channel reminders** (WhatsApp/SMS/e-mail)
* ✏️ **Digital intake & micro-check-ins** (mood scale, quick notes)
* 📊 **Progress tracker** showing attended vs planned sessions
* 🌐 **Responsive UI** (mobile-first, Tailwind CSS)
* 💾 Client-side data persistence via **browser localStorage** (no backend)

## Tech Stack

| Layer  | Tools                    |
| ------ | ------------------------ |
| UI     | HTML · Tailwind CSS      |
| Logic  | Vanilla JavaScript (ES6) |
| State  | localStorage + JSON      |
| Deploy | GitHub Pages             |

> Optionally, **Alpine.js** is included for lightweight reactivity—feel free to remove if you prefer pure JS.

## Getting Started

Clone the repo and run a local server (or just open `index.html`).

```bash
# 1. Clone
$ git clone https://github.com/rodrigomarquest/rorizlinhares.git
$ cd rorizlinhares

# 2. Serve (Option A – quick)
$ npx http-server -c-1                 # then open http://localhost:8080

# 2. Serve (Option B – VS Code Live Server)
# Install the Live Server extension, right-click index.html → "Open with Live Server"
```

## Project Structure

```
rorizlinhares/
├── assets/         # icons & images
├── css/
│   └── styles.css  # Tailwind build
├── js/
│   ├── store.js    # data layer (CRUD localStorage)
│   ├── ui.js       # DOM rendering helpers
│   └── reminders.js# scheduling logic
├── index.html      # SPA entry point
└── README.md       # this file
```

## Screenshots

Add screenshots to `/docs` and reference them here:

```md
![Home](docs/home.png)
![Booking Flow](docs/booking-flow.png)
```

## Roadmap

* Integrate Google Calendar API for two-way sync
* Persist data to Firebase or Supabase
* Add therapist dashboard with engagement metrics
* Implement push notifications (PWA)

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

Released under the **MIT License**. See `LICENSE` for details.

---

> **Disclaimer:** This prototype is for academic purposes only; no production patient data is stored or processed.
