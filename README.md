# <p align="center">Hey, I'm Anush Vishwakarma 👋</p>

<p align="center">
  <b>Backend Software Engineer & Open Source Contributor</b><br>
  Focused on High-Concurrency Systems, Distributed Caching, and Core Numerical Computing.
</p>

<p align="center">
  <a href="https://linkedin.com/in/anush-vishwakarma-98a8b7276/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://codeforces.com/profile/DE4d_B0dy"><img src="https://img.shields.io/badge/Codeforces-Specialist_(1414)-1F8ACB?style=flat-square&logo=codeforces&logoColor=white" alt="Codeforces" /></a>
  <a href="https://www.codechef.com/users/vishwakarmaa14"><img src="https://img.shields.io/badge/CodeChef-4★_(1813)-5B4638?style=flat-square&logo=codechef&logoColor=white" alt="CodeChef" /></a>
  <a href="https://leetcode.com/u/vishwakarmat914/"><img src="https://img.shields.io/badge/LeetCode-Profile-FFA116?style=flat-square&logo=leetcode&logoColor=white" alt="LeetCode" /></a>
  <a href="mailto:vishwakarmat914@gmail.com"><img src="https://img.shields.io/badge/Email-vishwakarmat914%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

---

### 🌐 Open Source Contributions

Active contributor to foundational Python scientific computing libraries:

- **[NumPy (NumFOCUS)](https://github.com/numpy/numpy)**
  - **[PR #33049](https://github.com/numpy/numpy/pull/33049)**: `BUG: include dtype class in finfo cache key to avoid aliasing (gh-32947)`
    - Fixed a critical floating-point cache aliasing bug in `numpy/_core` on platforms where `sizeof(longdouble) == sizeof(double)` (MSVC Windows & macOS ARM64).
    - Isolated cache keys by `(dtype, type(dtype))` and implemented regression test suites in `numpy/_core/tests/test_getlimits.py` to prevent silent float promotion and numerical instability across downstream libraries (`statsmodels`, `NiMARE`).
  - **[PR #32575](https://github.com/numpy/numpy/pull/32575)**: `DOC, TYPING: np.nan_to_num copy semantics and overloads (gh-29045)`
    - Standardized `np.nan_to_num` copy parameter semantics, `ValueError` exception boundaries, and reference returns for NumPy 2.0+.
    - Expanded static typing stub overloads in `numpy/lib/_type_check_impl.pyi` to enforce strict consistency between the runtime API and static type checkers.

---

### 💼 Work Experience

- **Software Engineer Intern** @ **Perceptive Labs** *(Jun 2026 – Sep 2026)*
  - **KhataClerk Reconciliation**: Developed the balance reconciliation engine matching vouchers across **1,000+ records** between Tally ERP and Zoho, handling complex multi-tier tax and ledger rounding edge cases.
  - **LLM Technical Interviewer**: Engineered an LLM-powered adaptive evaluation service across **150+ candidate sessions**, issuing pre-signed S3 URLs for direct client-to-cloud media chunk uploads to offload server bandwidth.
  - **Throughput Optimization**: Refactored candidate screening pipeline to execute across parallel **Celery + Redis** worker pools, slashing evaluation latency from **45s to 8s** per batch.
  - **Cloud Infrastructure**: Containerized microservices using **Docker** and established automated CI/CD deployment pipelines to **Google Cloud Run** backed by Cloud SQL.

---

### 🚀 Featured Engineering Projects

<table>
  <tr>
    <td width="50%">
      <h3 align="center"><a href="https://github.com/Rvish-glitch/api-rate-limiter">RateShield</a></h3>
      <p align="center"><b>Distributed API Gateway & Rate Limiter</b></p>
      <ul>
        <li>Reverse-proxy API Gateway built with <b>FastAPI</b> & Docker Compose with centralized JWT authentication and RBAC.</li>
        <li>Route-aware sliding-window rate limiting utilizing <b>Redis Sorted Sets (ZSET)</b> with dynamic <code>Retry-After</code> headers.</li>
        <li>Benchmarked with <b>Locust</b> under <b>500 concurrent simulated users</b>, sustaining <b>2,500+ req/sec</b> at sub-10ms latency.</li>
        <li>In-memory fallback cache with graceful degradation during Redis connection dropouts.</li>
      </ul>
      <p align="center">
        <code>FastAPI</code> • <code>Redis</code> • <code>PostgreSQL</code> • <code>Docker</code> • <code>Locust</code>
      </p>
    </td>
    <td width="50%">
      <h3 align="center"><a href="https://github.com/Rvish-glitch/streamdocs">StreamDocs</a></h3>
      <p align="center"><b>Async Document Ingestion Platform</b></p>
      <ul>
        <li>Asynchronous document extraction pipeline offloading multipage PDF parsing tasks to background <b>Celery</b> workers.</li>
        <li>Worker stability hardened with isolated subprocesses, <b>30s soft-timeout</b> warning, and <b>35s SIGKILL hard-timeout</b> to abort hung tasks and reclaim memory.</li>
        <li>Real-time progress streaming (<code>Queued</code> → <code>Parsing</code> → <code>Completed</code>) via <b>Redis Pub/Sub</b> bridged into persistent WebSockets.</li>
        <li>Interactive dashboard in <b>React + TypeScript</b> with search, live progress, and multi-format export.</li>
      </ul>
      <p align="center">
        <code>FastAPI</code> • <code>Celery</code> • <code>Redis Pub/Sub</code> • <code>WebSockets</code> • <code>React</code>
      </p>
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <h3 align="center"><a href="https://github.com/Rvish-glitch/nutripy">NutriScan</a></h3>
      <p align="center"><b>Real-Time Nutrition & Ingredient Intelligence Platform</b></p>
      <ul>
        <li>Real-time barcode and QR code detection to scan and decode packaged food items into nutritional logging pipelines.</li>
        <li>Sub-millisecond query responses powered by an in-memory cache backed by indexed <b>SQLite</b> tables to eliminate redundant upstream calls.</li>
        <li>Interfaced Open Food Facts API for automated ingredient extraction; packaged via Docker for reproducible deployments.</li>
      </ul>
      <p align="center">
        <code>FastAPI</code> • <code>React.js</code> • <code>SQLite</code> • <code>Docker</code>
      </p>
    </td>
  </tr>
</table>

---

### 🏆 Competitive Programming & Achievements

- **Meta Hacker Cup 2025**: Ranked **1579** (Round 1) and **1944** (Round 2) globally out of 20,000+ competitors. ([Certificate](https://www.facebook.com/codingcompetitions/hacker-cup/2025/certificate/1149301186617740))
- **CodeChef**: Peak Rating of **1813 (4-Star)** ([@vishwakarmaa14](https://www.codechef.com/users/vishwakarmaa14))
- **Codeforces**: Peak Rating of **1414 (Specialist)** ([@DE4d_B0dy](https://codeforces.com/profile/DE4d_B0dy))
- **ICPC India Preliminary 2024**: Secured **All India Rank 921** among 10,000+ teams.

---

### 🛠️ Tech Stack & Architecture

<p align="left">
  <b>Languages:</b><br>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />
</p>

<p align="left">
  <b>Backend & Concurrency:</b><br>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white" />
  <img src="https://img.shields.io/badge/React.js-61DAFB?style=flat-square&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white" />
  <img src="https://img.shields.io/badge/WebSockets-010101?style=flat-square&logo=socketdotio&logoColor=white" />
  <img src="https://img.shields.io/badge/Gunicorn-499848?style=flat-square&logo=gunicorn&logoColor=white" />
</p>

<p align="left">
  <b>Databases & Caching:</b><br>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" />
</p>

<p align="left">
  <b>DevOps, Cloud & Systems:</b><br>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Google_Cloud_Run-4285F4?style=flat-square&logo=googlecloud&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
</p>

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Rvish-glitch&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="165" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Rvish-glitch&layout=compact&theme=tokyonight&hide_border=true" height="165" />
</p>

<p align="center">
  <i>Feel free to explore my repositories, check out the PRs, or connect for collaborations!</i>
</p>
