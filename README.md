<div align="center">

<img src="./assets/banner.gif" alt="Ziad: pixel-art scene of a rover scanning a stressed plant" width="100%" />

```text
 ███████╗██╗ █████╗ ██████╗
 ╚══███╔╝██║██╔══██╗██╔══██╗     Ziad Emad Salem
   ███╔╝ ██║███████║██║  ██║     ──────────────────────────────
  ███╔╝  ██║██╔══██║██║  ██║     applied AI · robots · algorithms
 ███████╗██║██║  ██║██████╔╝     Grade 12 · Giza, Egypt
 ╚══════╝╚═╝╚═╝  ╚═╝╚═════╝      ISEF finalist · ACPC Top 31
```

[![Portfolio](https://img.shields.io/badge/portfolio-open-3fb950?style=flat-square&logo=vercel&logoColor=white)](https://portfolio-2kkf.vercel.app/)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0001--7460--1592-a6ce39?style=flat-square&logo=orcid&logoColor=white)](https://orcid.org/0009-0001-7460-1592)

</div>

---

### `$ dmesg | tail` — what I'm made of

```text
[    0.001] curiosity        loaded      (no unload routine found)
[    0.042] python 3.12      ready       pytorch · opencv · mediapipe · fastapi
[    0.077] c++              ready       competitive programming, embedded
[    0.103] esp32-cam        attached    /dev/rover0, streaming
[    0.150] bio-signal       calibrated  sEMG + VOC arrays, plants as sensors
[    0.201] school           STEM 6th of October, 98% entry score, rank 245 nationally
[    0.256] goal             B.Sc. + research in AI & Computer Engineering
[    0.300] mood             compiling
```

---

### `$ cd projects/` — click a folder

<details>
<summary><b>📁 aether/</b> &nbsp;·&nbsp; plants that raise their own alarm &nbsp;·&nbsp; <i>ISEF Egypt National Finalist</i></summary>

<br/>

A crop under attack changes its electrical signature and its scent before a human can see anything. **AETHER ("The Pytho Sentry")** reads both, then lets deep learning decide whether the plant is fine or in trouble. I was the AI-modeling director and lead developer.

```text
 plant ──► sEMG electrodes ─┐
                            ├─► 1D CNN  ─┐
 leaf  ──► VOC sensor array ┤            ├─► fuse ─► [ HEALTHY | STRESSED | PEST ]
                            └─► 2D CNN  ─┘

 healthy   ▁▁▂▂▁▁▂▃▂▁▁▂▂▁▁▂▂▁▁▂▁▁▂▂▁▁
 stressed  ▁▂▅█▇▃▁▂▆█▅▂▁▃▇█▆▂▁▂▅█▇▃▁▂
                ▲ alarm
```

`PyTorch` `1D/2D CNN` `Bio-signal processing` `Sensor fusion`

</details>

<details>
<summary><b>📁 pipe-rover/</b> &nbsp;·&nbsp; six wheels, one camera, zero humans in the pipe</summary>

<br/>

A compact 6WD robot that drives into pipelines too tight or too dangerous for people, streams live video, and sniffs for gas. Driven from a wireless web UI.

```text
    ┌─────────────────────────┐
 ◉═╡ ESP32-CAM  ◉  live feed  ╞═◉
 ◉═╡ MQ-2 gas   ░░░░  HC-SR04 ╞═◉
 ◉═╡ L298N ▓▓▓▓▓▓▓▓ L298N     ╞═◉
    │ 18650 ███ SG90 pan/tilt │
    └─────────────────────────┘
```

`ESP32-CAM` `2× L298N` `MQ-2` `HC-SR04` `SG90 pan/tilt` `18650 power` `web control UI`

</details>

<details>
<summary><b>📁 dark-night/</b> &nbsp;·&nbsp; a Halloween platformer with my own physics</summary>

<br/>

Pure Python and Pygame, no engine. Custom physics, and packaged as standalone builds for Windows, Linux and macOS.

```text
                     ,-.            *        .
        .           ( ☾ )     .          *
              *      `-'          .
   .                                  .        ☠
              🎃            ▄▄▄▄▄▄▄▄          ▄▄▄▄
   ▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄          ▀▀▀▀▀▀▀▀      ▄▄▄▀▀▀▀▀
```

`Python` `Pygame` `custom physics` `cross-platform builds`

</details>

<details>
<summary><b>📁 realtime-vision/</b> &nbsp;·&nbsp; webcam detection and AI agents</summary>

<br/>

Optimizing live webcam object detection with **RF-DETR + Supervision**, and wiring agent workflows and bots with LangChain, FastAPI, n8n, LiveKit Cloud and the Telegram API.

`RF-DETR` `Supervision` `LangChain` `n8n` `LiveKit` `OpenRouter`

</details>

---

### `$ cat fenwick.cpp` — how my head works in contests

```cpp
// prefix sums that can change: O(log n) update, O(log n) query
struct Fenwick {
    int n; vector<long long> t;
    Fenwick(int n) : n(n), t(n + 1, 0) {}
    void add(int i, long long v) { for (; i <= n; i += i & -i) t[i] += v; }
    long long sum(int i) { long long s = 0; for (; i > 0; i -= i & -i) s += t[i]; return s; }
};
// also in my toolbox: sparse tables, prefix sums, graphs, trees, DP
```

---

### `$ ./trophies --verbose`

```diff
+ [✔] ISEF Egypt ............. National Finalist, Project AETHER
+ [✔] ACPC ................... Africa & Arab Collegiate Programming Championship, Top 31
+ [✔] NASA Space Apps Giza ... "Galactic Problem Solver"
+ [✔] The Earth Prize ........ global participant, sustainable engineering proposal
```

<details>
<summary><b>$ whoami --leadership</b></summary>

<br/>

| Role | Where |
|---|---|
| Head of Machine Learning & IT | Model Arab League: wrote the curriculum, ran the Python, data structures and ML-roadmap workshops |
| President | High School Aviation & Aerospace Club |
| Team Leader | Resala STEM Volunteering Team |
| Member | Hack Club, logging build hours with Hackatime |

</details>

<details>
<summary><b>$ pip freeze</b></summary>

<br/>

```text
languages      Python 3.12 · C++ · C/Arduino · HTML/CSS/JS · Markdown
ml / cv        PyTorch · scikit-learn · OpenCV · MediaPipe · RF-DETR · Supervision
data           NumPy · Pandas · Matplotlib · Seaborn
backend/agents FastAPI · LangChain · n8n · LiveKit Cloud · OpenRouter API
hardware       ESP32 / ESP32-CAM · Arduino Uno · Raspberry Pi · relays · motor drivers · power mgmt
apps           Pygame · Tkinter
workflow       Linux · Windows · Git & GitHub
```

</details>

<details>
<summary><b>$ git log --stat</b></summary>

<br/>

<img src="https://github-readme-stats.vercel.app/api?username=ziad-emad-salem&show_icons=true&theme=dark&hide_border=true&bg_color=0d1117&title_color=3fb950&icon_color=58a6ff&text_color=c9d1d9" alt="github stats" />

</details>

---

<div align="center">

```text
$ ./contact.sh
> open to research, internships and building real AI systems
> portfolio : portfolio-2kkf.vercel.app
> orcid     : 0009-0001-7460-1592
$ echo "the best model is the next one you train"
the best model is the next one you train
$ _
```

</div>
