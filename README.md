# 🎭 Crooked Smile — Face Prompt Builder

> Free, offline, **single-file** HTML app for building image-generation prompts of realistic, naturally asymmetrical female faces.

[![Single file](https://img.shields.io/badge/Single%20file-HTML-2563eb)]() [![100% offline](https://img.shields.io/badge/Offline-100%25-16a34a)]() [![No install](https://img.shields.io/badge/Install-None-f59e0b)]()

![Crooked Smile — Face Prompt Builder](assets/screenshot.png)

## What is it?

Pick options across **17 sections** — face shape, hair, eyes, cosmetics, style & vibe, lighting, camera, head pose… — and the app assembles a detailed **English prompt** for image models (Stable Diffusion, Krea 2 and modern image LLMs). **474 hand-drawn icons** make every option visible at a glance, so you can build a face the way you'd describe it to an artist.

## Quick start

1. Grab `face_prompt_builder_offline_v2.html` (download or clone this repo)
2. Open it in any modern browser — Chrome, Firefox, Safari, Edge
3. Pick options (or roll the 🎲), copy the prompt, paste it into your image tool

No server. No internet. No account. No install.

## Features

- **17 sections, 474 icon options** — single- and multi-select, every category can be bypassed with one click
- **🎲 Random roll** — re-roll everything, or fill only the empty slots while your picks stay pinned
- **✍️ Krea-2 optimizer** — rewrites the tag list as a natural-language scene description
- **🔁 Reverse engineer** — paste your own English face prompt and the app maps it onto its own vocabulary (via a local LLM, e.g. LM Studio)
- **💾 Saved recipes** — unlimited presets, stored on your device
- **🧊 3D head-pose preview**
- **🌍 6 UI languages** (EN, DE, FR, ES, RU, ZH) — the generated prompt is always English
- **🌑 Light & dark mode**

## Requirements

- A modern web browser — that's it
- *Optional:* [LM Studio](https://lmstudio.ai) or any OpenAI-compatible local API, only for the reverse-engineer mode

All faces are fictional adults (18+); the app never depicts real people.

## Status

**V2 — stable.** All 17 sections ship with full icon coverage; everything runs offline. Actively maintained — issues and PRs welcome.

## License

Free for personal, hobby and student use — **not licensed for commercial use**.
