<div align="center">

# ClipShow.ai

### The Enterprise-Grade, 100% Free & Open-Source Multi-Modal Highlight & Virality Engine for Long-Form Streams

**Transform 1-hour to 40-hour live streams and VODs into high-converting 9:16 vertical shorts in seconds.**  
**Zero GPU Required • 8 GB RAM Safe • Zero Cloud API Costs • 100% Local & Private**

---

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Python 3.12](https://img.shields.io/badge/Python-3.12-3776AB.svg?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688.svg?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![React 19](https://img.shields.io/badge/Frontend-React_19-61DAFB.svg?style=for-the-badge&logo=react&logoColor=black)](https://react.dev)
[![Vite](https://img.shields.io/badge/Build-Vite-646CFF.svg?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev)
[![TailwindCSS v4](https://img.shields.io/badge/UI-TailwindCSS_v4-38B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com)
[![FFmpeg Accelerated](https://img.shields.io/badge/Engine-FFmpeg_UltraFast-007808.svg?style=for-the-badge&logo=ffmpeg&logoColor=white)](https://ffmpeg.org)
[![Platform Independence](https://img.shields.io/badge/Architecture-CPU_Only_Ready-orange.svg?style=for-the-badge)](#system-architecture)

---

### [ STAR THIS REPOSITORY TO BE NOTIFIED THE EXACT SECOND THE FULL CODEBASE DROPS ]

*Codebase drop in progress. Star the repo and watch releases to get immediate 1-click access upon launch.*

---

</div>

## The Mission

Commercial highlight tools (such as Opus Clip, Munch, Klap, and Vidyo) charge steep monthly subscriptions, enforce strict upload duration limits, crash on multi-hour gaming streams, and lock your content into proprietary cloud silos.

**ClipShow.ai is built to disrupt this model.**

ClipShow.ai is a fully autonomous, local-first virality suite engineered from scratch to analyze **massive streams (1 to 40+ hours)** with mathematical precision, frame-accurate lip sync, and professional Premiere Pro-grade editing controls—running entirely on commodity consumer hardware with **$0 cloud fees**.

---

## Key Breakthroughs & Capabilities

### 1. Multi-Modal Virality Physics Engine (4-Signal Fusion)
ClipShow.ai does not rely on naive text summarization or uniform interval slicing. It extracts and fuses four independent telemetry signals into a rolling normalized virality score:

* **Signal A: Crowd Retention & Heatmap Curves**  
  Captures real audience rewatch spikes, retention peaks, and organic viewer re-engagement.
* **Signal B: Live Chat Velocity Bursts & Sentiment Momentum**  
  Parses high-density chat message frequency, emote bursts, and sudden reaction surges with sub-second temporal resolution.
* **Signal C: 8 kHz Vocal Acoustic Physics (Scream Spikes & Silent Clutch Dynamics)**  
  Analyzes human vocal frequency bands (300 Hz to 3400 Hz) to identify hype screams, shoutcaster moments, and silent clutch build-ups followed by explosive reactions.
* **Signal D: Micro-Visual Scene Transitions & Motion Deltas**  
  Scans keyframe I-frame transitions and rapid combat cuts without decoding unneeded intermediate frames.

### 2. Hierarchical Stratified Non-Maximum Suppression (NMS)
* **Zero Timestamp Clustering:** Standard peak detectors cluster around a single 5-minute loud sequence. ClipShow.ai applies dynamic exclusion radii that adapt mathematically to video duration.
* **Narrative Arc Distribution:** Guarantees highlight diversity across every phase of the broadcast (Opening Hype -> Mid-Game Tension -> Climax -> Ending Reaction).
* **Guaranteed Output Delivery:** Whether analyzing an intense tournament or a calm 8-hour stream, the stratified anchor algorithm guarantees delivery of your exact requested clip count (e.g. 4, 8, 12, or 24 shorts).

### 3. Sub-20-Second Time-to-First-Clip (Turbo SSE Pipeline)
* **Progressive Server-Sent Events (SSE):** Rather than forcing creators to wait hours for a 10-hour VOD to process:
  * **Batch 1 (Instant Highlights):** Delivers the top 4 instant highlights in approximately 15 to 20 seconds.
  * **Batch 2 (Background Refinement):** Delivers remaining highlights progressively while you begin editing immediately.

### 4. Full Premiere Pro-Grade 9:16 Video Studio
ClipShow.ai includes a built-in browser-based workstation:
* **Multi-Region Compositing:** Instant dynamic split-screen layout (Facecam / Webcam Top + Gameplay Bottom) with customizable border colors and divider controls.
* **Interactive Pan & Zoom:** Drag-and-drop viewport adjustments on individual video slots directly inside the composition canvas.
* **Word-by-Word Kinetic Bounce Subtitles:** Real-time subtitle generator with custom color themes, stroke weights, active word glow, and bounce physics.
* **Multi-Track Timeline:** Dedicated tracks for video clips, audio tracks, text overlays, and subtitle cards with trimming, snapping, and undo/redo history.
* **Instant MP4 Export:** Produces clean, web-optimized H.264 `yuv420p` vertical videos with AAC stereo audio and hardware acceleration.

---

## Comparison Matrix

| Capability | ClipShow.ai | Opus Clip | Klap / Munch Studio | Traditional Editors |
| :--- | :--- | :--- | :--- | :--- |
| **Pricing & Quotas** | **100% Free & Unlimited Hours** | $0–$29/mo (Capped at 1–5 hrs/mo) | $29–$398/mo (Clip/minute caps) | $20–$50/mo |
| **Max Stream Duration** | **40+ Hours (No Upload Wait)** | Up to 10 Hours (Cloud Upload) | Up to 3 Hours | Manual Scrubbing |
| **Hardware Requirement** | **Intel CPU (8 GB RAM, No GPU)** | Cloud GPU Servers | Cloud GPU Servers | High-End GPU Rig |
| **Signal Modalities** | **Heatmap + Live Chat + Audio + Visual** | Visual + Audio + Transcript | Transcript + Audio/Visual | Manual Markers |
| **40h Anti-Clustering** | **Hierarchical Stratified NMS** | Standard Virality Ranking | Standard AI Ranking | Manual Timeline |
| **Time to First Clip** | **Sub-20 Seconds (Live SSE)** | 5–15 Minutes (Queue + Upload) | 10–20 Minutes | Hours |
| **Privacy & Sovereignty** | **100% Local / Self-Hosted** | Closed Cloud | Closed Cloud | Local |
| **Built-in 9:16 Studio** | **Yes (Multi-Track + Split-Screen)** | Web Editor + XML Export | Web Editor | Full NLE (Manual Setup) |
| **License** | **MIT License (Open Source)** | Proprietary SaaS | Proprietary SaaS | Proprietary Software |

---

## System Architecture

```
[ Raw Stream / VOD / Local MP4 ] (1h to 40h+)
                │
                ├──> Stage 1: Streaming Feature Extraction (<300 MB RAM)
                │       ├── Signal A: Retention Heatmap Telemetry
                │       ├── Signal B: Chat Message Velocity Array
                │       ├── Signal C: 8 kHz Narrowband Acoustic Physics
                │       └── Signal D: Keyframe Scene & Motion Delta
                │
                ├──> Stage 2: Dynamic Rolling Z-Score Normalization
                │       └── Win: 600s Local Window | Zero-Variance NaN Guard
                │
                ├──> Stage 3: Stratified Hierarchical NMS Engine
                │       ├── Dynamic Exclusion Radius (T_video / (2 * N_target))
                │       └── Chapter-Balanced Anchor Allocation
                │
                ├──> Stage 4: Frame-Accurate Boundary Snapping & Dual Muxing
                │       ├── Acoustic Silence Snapping (Speech Boundary Lock)
                │       └── UltraFast H.264 yuv420p + AAC Stereo Assembly
                │
                └──> Live Studio Workspace (React 19 + Vite + Tailwind v4)
                        ├── Progressive SSE Stream Feed (Instant Batch 1 Delivery)
                        ├── Multi-Track Timeline & Audio Waveform Visualizer
                        ├── Smart Split-Screen Re-framing (Facecam + Gameplay)
                        └── Kinetic Animated Subtitles & 9:16 Exporter
```

---

## Resource & Hardware Specs

ClipShow.ai is explicitly engineered for accessibility:
* **Operating System:** Windows 10/11, macOS (Apple Silicon & Intel), Ubuntu / Debian Linux.
* **Minimum Processor:** Quad-core Intel Core i5 / AMD Ryzen 3 (or higher).
* **RAM Footprint:** Strictly under 300 MB peak Python RAM consumption during multi-hour scans.
* **Storage Requirement:** Lightweight streaming chunks; temporary storage cleaned automatically.
* **GPU Requirement:** **None.** Complete CPU optimization via FFmpeg threading and NumPy vectorized operations.

---

## Launch Roadmap

* [x] **Core Multi-Modal Engine Architecture** (Signals A through D verified).
* [x] **Stratified Hierarchical NMS** with dynamic temporal exclusion.
* [x] **Sub-20s Progressive SSE Streaming** pipeline.
* [x] **Premiere Pro-Grade 9:16 Workstation** with multi-track timeline and split compositing.
* [x] **Lip-Sync UltraFast Extraction** with web-standard `yuv420p` H.264 encoding.
* [ ] **One-Click Docker Compose & Binary Release** (In Progress).
* [ ] **Community Plugin Ecosystem** (Custom Subtitle Animation Presets & Voice AI Integration).
* [ ] **Public Codebase Drop (Free & Open Source)** (Imminent).

---

## How to Stay Updated

1. **Star this repository:** Click the star button in the upper right corner to get immediate notifications.
2. **Watch releases:** Enable Notifications -> Releases to receive the 1-click installer and source package the moment it is pushed.
3. **Share with Creators & Developers:** Help bring open-source autonomy to content creation.

---

## License

ClipShow.ai will be released under the **MIT License**. Free for personal, commercial, and enterprise deployment.

---

<div align="center">

**Built for creators, streamers, and developers worldwide.**  
*Stay tuned. The revolution in autonomous stream highlight extraction begins here.*

</div>
