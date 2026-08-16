## Resume Forge API

Resume Forge is a backend REST API powering a resume and CV building platform. It's built on **Node.js** and **Express**, following a clean, layered structure (`routes → controllers → models`). The project uses a lightweight file-based JSON store as its database, so no external database installation is needed to get it running or to test it.


## Introduction

With Resume Forge, a user can create an account, build out any number of resumes and cover letters, and organize the content of each into structured sections — Experience, Education, Skills, Projects, and more. Every document can be versioned (saved and rolled back), enhanced with lightweight AI writing suggestions, and linked to job applications the user is tracking.

This project was developed as part of a backend engineering course, emphasizing solid REST design, clear separation of concerns, and predictable, consistent responses across every route.

---

## Core Capabilities

- **Authentication** — Sign up, sign in, sign out, and recover a forgotten password, all backed by mock bearer-token sessions.
- **Account Management** — Retrieve, edit, or delete your own user profile.
- **Documents** — Create, read, update, and delete resumes/cover letters, with support for duplicating and importing them.
- **Sections & Items** — Attach ordered sections to a document (Experience, Education, Skills, Projects, Custom), each holding one or more flexible-field items.
- **Version Snapshots** — Capture a document's state at a given moment and revert to it later.
- **Template Browsing** — View templates made publicly available on the platform.
- **AI-Assisted Writing** — Refine bullet points and summaries, rewrite general text, or run a custom prompt against a section — each call draws from a per-user AI credit balance.
- **Application Tracker** — Record job applications tied to a specific resume and follow their status through applied, interviewing, offered, or rejected.
- **Uniform Responses** — Every route replies with the same `{ success, message, data }` envelope.

---

## Technologies Used

| Layer            | Tool/Tech                            |
|-------------------|--------------------------------------|
| Runtime           | Node.js                              |
| Web Framework     | Express.js                           |
| Storage           | JSON file (`data.json`)              |
| Auth Mechanism    | Mock Bearer token sessions           |
| API Testing Tool  | Postman                              |

---
