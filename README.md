# Parth Saini

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=1000&color=6366F1&center=true&vCenter=true&random=false&width=900&lines=Backend+%C2%B7+Systems+%C2%B7+AI%2FML+Engineer+@+IIT+Roorkee;SDE+Intern+@+Deutsche+Bank+%7C+Distributed+Systems;C%2B%2B+%C2%B7+Java+%C2%B7+Python+%C2%B7+Spring+Boot+%C2%B7+ZooKeeper;Dean+Academic+Award+2024+%7C+IIT+Roorkee" alt="Typing SVG" />
</div>

Backend, systems, and AI/ML engineer. Final year at IIT Roorkee.

I build things that have to handle real load: in-memory databases, distributed coordination systems, REST APIs that don't fall over. I also work across data pipelines and ML systems. I care about correctness, performance, and writing code that's actually maintainable.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/parthsaini2004/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:parth_s@mt.iitr.ac.in)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=flat-square&logo=leetcode&logoColor=white)](https://leetcode.com/parthsaini2004/)
![Profile Views](https://komarev.com/ghpvc/?username=parthsaini2004&style=flat-square&color=6366f1)

---

## Core Expertise

- **Systems Programming** -- concurrent data structures, lock-free design, event-driven I/O
- **Distributed Systems** -- leader election, fault tolerance, state synchronization, consensus
- **Backend Engineering** -- REST APIs, service architecture, database design, Spring Boot
- **AI and ML** -- recommendation systems, NLP pipelines, data analytics, scikit-learn, OpenAI API
- **CS Fundamentals** -- OS, DBMS internals, networking, data structures and algorithms

---

## Tech Stack

**Languages**

![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![HTML](https://img.shields.io/badge/HTML-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?style=flat-square&logo=css3&logoColor=white)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white)

**Frameworks and Infrastructure**

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Apache ZooKeeper](https://img.shields.io/badge/ZooKeeper-E4B84D?style=flat-square&logo=apache&logoColor=black)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=flat-square&logo=hibernate&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)

**Data and ML**

![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![OpenAI API](https://img.shields.io/badge/OpenAI_API-412991?style=flat-square&logo=openai&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

**Tools**

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**Coursework:** Data Structures and Algorithms, OOP, DBMS, Operating Systems, Computer Networks, Web Development, Data Analytics

---

## Projects

### FlashKV -- High-Performance In-Memory Key-Value Store

Redis-compatible KV store written in C++ from scratch. The goal was to understand what actually makes Redis fast.

- Event-driven networking model on a single thread, handling 10,000+ concurrent client connections without spawning a thread per connection
- Storage engine partitioned into 32 independent shards with reader-writer locks for parallel request execution -- scales to ~120,000 ops/sec
- Append-only disk persistence for crash recovery; bounded-queue backpressure to prevent memory exhaustion under spike loads

`C++` `Event-driven I/O` `Concurrent data structures` `Redis RESP protocol`

---

### Distributed Server Coordination System -- Deutsche Bank

Built during my internship at Deutsche Bank. The problem: make a cluster of servers coordinate without any single point of failure.

- Servers self-register, elect a leader via ZooKeeper, monitor each other's health, and handle node failures automatically
- Leader-based write pipeline with unified state synchronization across the cluster -- consistent behavior regardless of which node handles a request
- Integrated the coordination layer with both server-side and client-side architecture so the system adapts dynamically as nodes join or leave

`Java` `Spring Boot` `Apache ZooKeeper` `PostgreSQL` `Hibernate` `JPA` `JDBC`

---

### Movie Recommendation System

Context-aware recommendation engine built with a multi-hot feature vector approach and cosine similarity for Top-K suggestions.

- Converts movies into multi-hot and numerical feature vectors; computes cosine similarity for session-aware Top-K results
- TMDB metadata integration via Node.js API + MongoDB event store for real-time user interaction tracking
- Modular full-stack architecture: Python similarity engine, Node.js backend, React frontend

`Python` `Node.js` `MongoDB` `React` `REST APIs`

---

### Customer Support ChatBot System

AI-powered order support assistant for e-commerce workflows.

- Node.js backend with intent-aware routing and REST workflows connected to order data -- users can query delivery status, delays, and refund eligibility through a single conversational interface
- React frontend + Python order services with axios request flows, message handling, and validation pipelines
- Supports order tracking, password management, and user request handling end-to-end

`Node.js` `React` `Python` `OpenAI API` `REST APIs`

---

### IARC Website -- Institute Alumni Relations Cell, IIT Roorkee

Full-stack alumni engagement platform for IIT Roorkee built in collaboration with the Dean (DORA).

- Enables alumni updates, reunion registrations, event participation, and donation workflows
- Translated institute goals into platform features; implemented communication and engagement modules used by the wider alumni network

`React` `Node.js` `Full-stack`

---

## Experience

**Software Engineering Intern -- Deutsche Bank** `June 2025 - July 2025` | Pune

Worked on distributed systems infrastructure. Built the server coordination system described above. The core challenge was making the cluster behave predictably under failure scenarios -- nodes leaving mid-transaction, split-brain edge cases, leader re-election timing.

Stack: Java, Spring Boot, Apache ZooKeeper, Hibernate, JPA, JDBC, PostgreSQL, React.js

---

**Frontend Developer -- Eazeplace** `March 2024 - June 2024` | Rishikesh

Built a full-stack internship/project matchmaking platform. Designed pre-verification workflows for candidate resumes and integrated recommendation logic for student-to-internship matching.

Stack: React.js, Node.js

---

## Education

**IIT Roorkee** | 2022 -- 2026

CGPA: 8.86/10

---

## Achievements and Leadership

- **Dean Academic Award (2024)** -- Awarded among 10,000+ students for academic performance
- **Joint Secretary (Web Development), IARC** -- Contributed to institute web platforms; organized alumni events, hackathons, and reunions

---

## GitHub Stats

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=parthsaini2004&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=6366f1&icon_color=6366f1&text_color=c9d1d9" width="49%" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=parthsaini2004&theme=github-dark-blue&hide_border=true&background=0d1117&ring=6366f1&fire=6366f1&currStreakLabel=6366f1" width="49%" />
</div>

---

<sub>IIT Roorkee &middot; Backend &middot; Systems Engineering &middot; Distributed Systems</sub>
