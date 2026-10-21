# <p align="center">Hi there, I'm Anush Vishwakarma 👋</p>

<p align="center">
  <b>Backend Engineer & Open Source Contributor</b><br>
  Building high-throughput APIs, distributed caching layers, and contributing to core Python scientific libraries.
</p>

<p align="center">
  <a href="https://linkedin.com/in/anush-vishwakarma-98a8b7276/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://codeforces.com/profile/DE4d_B0dy"><img src="https://img.shields.io/badge/Codeforces-Specialist-1F8ACB?style=flat-square&logo=codeforces&logoColor=white" alt="Codeforces" /></a>
  <a href="https://www.codechef.com/users/vishwakarmaa14"><img src="https://img.shields.io/badge/CodeChef-4★-5B4638?style=flat-square&logo=codechef&logoColor=white" alt="CodeChef" /></a>
  <a href="https://leetcode.com/u/vishwakarmat914/"><img src="https://img.shields.io/badge/LeetCode-Profile-FFA116?style=flat-square&logo=leetcode&logoColor=white" alt="LeetCode" /></a>
  <a href="mailto:vishwakarmat914@gmail.com"><img src="https://img.shields.io/badge/Email-vishwakarmat914%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

---

### 🌐 Open Source Contributions

Active merged contributor to foundational numerical computing libraries:

- **[numpy / numpy](https://github.com/numpy/numpy)**
  - **[PR #33049](https://github.com/numpy/numpy/pull/33049)** `merged`: **BUG: include dtype class in finfo cache key to avoid aliasing (gh-32947)**
    - Fixed a floating-point cache aliasing issue in `numpy/_core` on platforms where `sizeof(longdouble) == sizeof(double)` (MSVC Windows & macOS ARM64).
    - Isolated cache keys by `(dtype, type(dtype))` and implemented regression tests in `test_getlimits.py` to prevent silent float promotion and downstream solver errors (`statsmodels`, `NiMARE`).
  - **[PR #32575](https://github.com/numpy/numpy/pull/32575)** `merged`: **DOC, TYPING: np.nan_to_num copy semantics and overloads (gh-29045)**
    - Standardized `np.nan_to_num` copy semantics and `ValueError` exception boundaries for NumPy 2.0+.
    - Updated static typing definitions and function overloads in `numpy/lib/_type_check_impl.pyi` to enforce runtime API consistency with type checkers.

---

### 🚀 Featured Repositories

<table>
  <tr>
    <td width="50%">
      <h3 align="center"><a href="https://github.com/Rvish-glitch/api-rate-limiter">⚡ RateShield</a></h3>
      <p align="center"><i>Distributed Reverse-Proxy Gateway & Rate Limiter</i></p>
      <ul>
        <li>Route-aware sliding-window rate limiting powered by <b>Redis Sorted Sets (ZSET)</b>.</li>
        <li>Benchmarked with <b>Locust</b> under 500 concurrent users at <b>2,500+ req/sec</b> (sub-10ms proxy latency).</li>
        <li>Centralized JWT authentication, RBAC, and in-memory graceful degradation fallback.</li>
      </ul>
      <p align="center">
        <img src="https://img.shields.io/badge/Python-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
        <img src="https://img.shields.io/badge/Redis-ZSET-DC382D?style=flat-square&logo=redis&logoColor=white" />
        <img src="https://img.shields.io/badge/Docker-Compose-2496ED?style=flat-square&logo=docker&logoColor=white" />
      </p>
    </td>
    <td width="50%">
      <h3 align="center"><a href="https://github.com/Rvish-glitch/streamdocs">📄 StreamDocs</a></h3>
      <p align="center"><i>Asynchronous Multi-Document Processing Platform</i></p>
      <ul>
        <li>Asynchronous PDF text extraction pipeline offloaded to background <b>Celery</b> workers.</li>
        <li>Worker stability enforced via isolated subprocesses with soft warnings and <b>SIGKILL hard timeouts</b>.</li>
        <li>Real-time progress streaming bridged from <b>Redis Pub/Sub</b> into persistent WebSockets.</li>
      </ul>
      <p align="center">
        <img src="https://img.shields.io/badge/FastAPI-Backend-009688?style=flat-square&logo=fastapi&logoColor=white" />
        <img src="https://img.shields.io/badge/Celery-Worker-37814A?style=flat-square&logo=celery&logoColor=white" />
        <img src="https://img.shields.io/badge/React-TypeScript-61DAFB?style=flat-square&logo=react&logoColor=black" />
      </p>
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <h3 align="center"><a href="https://github.com/Rvish-glitch/nutripy">🥗 NutriScan</a></h3>
      <p align="center"><i>Real-Time Barcode & Nutritional Intelligence Platform</i></p>
      <ul>
        <li>Instant barcode & QR code decoding pipeline mapped to Open Food Facts ingredient queries.</li>
        <li>Sub-millisecond query responses backed by an in-memory inverted cache with indexed <b>SQLite</b> tables.</li>
        <li>Containerized microservice architecture packaged via <b>Docker</b> for cloud deployment.</li>
      </ul>
      <p align="center">
        <img src="https://img.shields.io/badge/Python-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
        <img src="https://img.shields.io/badge/React.js-Frontend-61DAFB?style=flat-square&logo=react&logoColor=black" />
        <img src="https://img.shields.io/badge/SQLite-In--Memory-003B57?style=flat-square&logo=sqlite&logoColor=white" />
        <img src="https://img.shields.io/badge/Docker-Container-2496ED?style=flat-square&logo=docker&logoColor=white" />
      </p>
    </td>
  </tr>
</table>

---

### 🛠️ Languages & Technologies

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/React.js-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
</p>

---

### 📊 GitHub Activity & Metrics

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Rvish-glitch&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="165" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Rvish-glitch&layout=compact&theme=tokyonight&hide_border=true" height="165" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=Rvish-glitch&theme=tokyonight&hide_border=true" height="165" />
</p>
