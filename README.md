# GSoC 2026 Final Work Submission

**Contributor:** Fahd Ashour ([@fahdfady](https://github.com/fahdfady))

**Organization:** MetaCall

**Project:** Improve MetaSSR

**Mentor:** Jose, Param Siddharth, Mozammil Ali

**Project size:** Large (350 hours)

**Synopsis:**

**Contact:** <fahd.fady212@gmail.com> · [LinkedIn](https://linkedin.com/in/fahdashour)

---

## 1. Project Goals

MetaSSR already delivers fast SSR and does well on the benchmarks, which is promising. But the dev mode, tests, and error handling still need hardening to be production‑ready. This project aims to make MetaSSR more mature and production-ready, focusing on improving the API handler (the core idea of MetaSSR, Polyglot programming via MetaCall), stabilizing and adding feature to the dev mode, expanding tests, and improving CI/reporting and documentation. If needed, the work will include changes to the MetaCall Rust port to support MetaSSR reliability & maintainability.

## 2. What I Did

I implemented the Polyglot API handler and integrated it in the project in a crate `metassr-api-handler` using metacall for the first time effectively in this project. This crate also could be used separately and I plan to ship this crate independently for developers who would love to create polyglot backend APIs using MetaCall, and not be forced to use MetaSSR's frontend features.

Added Python and JavaScript as languages supported by the polyglot api handler.

Eventually letting me add a new example "Sales Dashboard" that lets us use numpy/pandas on the Python side, while still having a JavaScript endpoint.

Added config for MetaSSR `metassr.toml` to include persistent configuration for your projects instead of just CLI.

I also posted a couple of devlogs. I planned to post a lot more to document the journey but i think that's okay.

- <https://fahdashour.com/devlog/001-metassr-examples/>
- <https://fahdashour.com/devlog/002-metassr-functionmesh-integration/>

## 3. Current State

## 4. What's Left

Middleware. We actually didn't find any usecase for it yet, decided that when we actually need security stuff done by the middleware we'll implement it. there is an RFC.

dockerize

serialization

lockfree

## 5. Merged Pull Requests

## 6. Challenges & Lessons Learned

---
