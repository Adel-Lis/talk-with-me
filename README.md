# Talk With Me — AI Personal Assistant

![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-3776AB.svg?logo=python&logoColor=white) ![Gradio](https://img.shields.io/badge/Gradio-4+-orange?logo=gradio) ![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4o--mini-412991?logo=openai) ![HuggingFace](https://img.shields.io/badge/HuggingFace-Spaces-yellow?logo=huggingface) ![License](https://img.shields.io/badge/License-MIT-green)

This is my first Agentic Project, I have built a simple AI-powered personal Adel assistant that represents (the professional) me on the web. The UI was built with Gradio and the artificial mind behind is powered by GPT-4o-mini, it answers questions about my background, experience, and skills — as if you were talking to me directly.

## Demo

[Live on HuggingFace Spaces](https://huggingface.co/spaces/Adel13Lis/Talk_With_Me)

---

## Overview

| Feature           | Details                                                           |
| ----------------- | ----------------------------------------------------------------- |
| Conversational AI | Represents my professional background in a human, natural tone    |
| Grounded answers  | Based on my real LinkedIn profile and personal summary            |
| Avatar            | Profile picture displayed next to every AI response               |
| Starter questions | Clickable chips to help users get started                         |
| Contact recording | Automatically records interested users via Pushover notifications |
| Unknown questions | Unanswered questions are flagged and recorded for follow-up       |
| UI feedback       | Toast notifications and loading indicator for a smooth experience |
| Deployment        | Hosted on HuggingFace Spaces with GitHub Actions auto-deploy      |

---

## Local Setup

**1 — Clone the repo**

```bash
git clone https://github.com/YOUR_USERNAME/talk-with-me
cd talk-with-me
```

**2 — Install dependencies**

```bash
uv pip install -r requirements.txt
```

**3 — Add your secrets in a `.env` file**

```
OPENAI_API_KEY=your_openai_key
PUSHOVER_TOKEN=your_pushover_token
PUSHOVER_USER=your_pushover_user
```

**4 — Add your personal files in a `me/` folder**

```
me/
├── linkedin.pdf
├── summary.txt
└── picture_of_me.JPG
```

**5 — Run the app**

```bash
uv run app.py
```

---

## Deployment

This project is deployed on HuggingFace Spaces via GitHub Actions. Every push to `main` triggers an automatic redeploy.

Secrets are stored in HuggingFace Space settings and injected as environment variables at runtime.

> **Disclaimer:** The `me/` folder contains personal data (LinkedIn PDF, personal summary, profile picture) that is the exclusive property of Adel Lis. Any reproduction, distribution, or use without explicit written permission is strictly prohibited.

---

## License

MIT License — see [LICENSE](LICENSE) for details.

Code is freely reusable. Personal content in the `me/` folder (CV, photo, summary) is the exclusive property of Adel Lis and is not licensed for reuse.
