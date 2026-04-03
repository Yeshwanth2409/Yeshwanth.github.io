# Yeshwanth Satyadev Yedla — Portfolio Website

Personal portfolio website showcasing my experience as an **AI/ML Engineer**, built with HTML, CSS, JavaScript, and deployed via **GitHub Pages**.

**Live Site:** [yeshwanth2409.github.io](https://yeshwanth2409.github.io)

---

## Overview

A responsive, single-page portfolio featuring:

- **Hero Section** — Animated typing effect cycling through roles (AI/ML Engineer, Python Gen AI, Software Engineer)
- **About** — Profile summary, core skills with animated progress bars, and technical expertise
- **Resume** — Professional experience (Ford Motor Company, Seneca Global), education (Stevens Institute of Technology, VNR VJIET), and downloadable resume link
- **Projects** — Featured work including DEV 11 Fantasy Cricket Platform, Sales Data Pipeline, and Gmail Sentiment Analysis with Vertex AI
- **Contact** — Address, phone, email, and social links
- **Chat with YeshwanthAI** — An AI-powered chatbot that answers questions about my career and background in real time

---

## Chat with YeshwanthAI

A floating chatbot widget embedded in the bottom-right corner of the portfolio. It connects to a **Gradio** app hosted on [Hugging Face Spaces](https://huggingface.co/spaces/Yeshwanth240901/dev_chat1) and lets visitors ask questions about my experience, skills, and projects — as if they were talking directly to me.

### How It Works

The chatbot is powered by a Python backend using **OpenAI's GPT-4o-mini** model with custom tool-calling capabilities:

```
User visits portfolio
        |
        v
Clicks "Chat with YeshwanthAI" button
        |
        v
Gradio chat UI loads in an iframe
        |
        v
User asks a question
        |
        v
GPT-4o-mini responds in-character as Yeshwanth,
using my LinkedIn profile + summary as context
        |
        v
If the user shares their email --> record_user_details tool fires
If a question can't be answered --> record_unknown_question tool fires
```

### Key Features

| Feature | Description |
|---|---|
| **In-character responses** | The AI represents me faithfully using my resume, LinkedIn profile, and a curated summary as context |
| **Tool calling** | Two function tools — `record_user_details` (captures visitor emails/names) and `record_unknown_question` (logs unanswered questions for review) |
| **Push notifications** | Every recorded email or unknown question triggers a real-time push notification via **Pushover API**, so I never miss a lead |
| **Conversation steering** | The system prompt guides visitors toward sharing their email for follow-up |

### Tech Stack (Chatbot)

- **Model:** OpenAI GPT-4o-mini with function calling
- **Backend:** Python, OpenAI SDK, pypdf, python-dotenv
- **Frontend:** Gradio ChatInterface
- **Hosting:** Hugging Face Spaces
- **Notifications:** Pushover API
- **Integration:** Embedded as an iframe in the portfolio

---

## Tech Stack (Portfolio)

| Layer | Technologies |
|---|---|
| **Frontend** | HTML5, CSS3, JavaScript, Bootstrap 4 |
| **Fonts** | Google Fonts (Poppins) |
| **Animations** | AOS (Animate On Scroll), Owl Carousel, custom CSS keyframes |
| **Icons** | Ionicons, Flaticon, IcoMoon, Open Iconic |
| **Hosting** | GitHub Pages |

---

## Project Structure

```
Yeshwanth.github.io/
├── index.html          # Main portfolio page (single-page app)
├── css/
│   ├── style.css       # Primary stylesheet (Bootstrap + custom theme)
│   ├── animate.css     # Animation library
│   ├── aos.css         # Animate On Scroll styles
│   └── ...             # Icon and component stylesheets
├── js/
│   ├── main.js         # Core site logic
│   ├── jquery.min.js   # jQuery
│   └── ...             # Carousel, animations, scrolling plugins
├── images/             # Profile photo, project thumbnails, backgrounds
├── fonts/              # Icon font files
├── scss/               # SCSS source files
└── README.md
```

---

## Color Theme

The portfolio uses a **deep navy + vibrant purple/cyan** color scheme:

| Element | Color |
|---|---|
| Background | `#0a0a1a` (deep navy) |
| Primary accent | `#8b5cf6` (vivid purple) |
| Secondary accent | `#38bdf8` (electric cyan) |
| Text (body) | `#cbd5e1` (light slate) |
| Text (headings) | `#f1f5f9` (near white) |
| Muted text | `#94a3b8` (slate gray) |

---

## Running Locally

```bash
# Clone the repository
git clone https://github.com/Yeshwanth2409/Yeshwanth.github.io.git

# Open in browser
open index.html
```

No build step required — it's a static site.

---

## Contact

- **Email:** yyeshwanthsatyadev@gmail.com
- **LinkedIn:** [linkedin.com/in/yeshwanth-satyadev-y-2a5a81254](https://www.linkedin.com/in/yeshwanth-satyadev-y-2a5a81254/)
- **GitHub:** [github.com/Yeshwanth2409](https://github.com/Yeshwanth2409)
- **GCP Certification:** [Credly Badge](https://www.credly.com/badges/1b1af193-8689-4908-96d3-9f42bb6da490)

---

## License

This template is based on [Colorlib](https://colorlib.com) and is licensed under **CC BY 3.0**. Custom modifications and content are by Yeshwanth Satyadev Yedla.
