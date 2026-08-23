# Duc An Nguyen — Personal Portfolio

Personal portfolio website documenting my work in **computer vision, edge AI, explainable AI, and industrial AI systems**, together with technical notes and selected professional and personal experiences.

The website is built as a lightweight static site using **HTML, CSS, and JavaScript**, with an emphasis on clear technical communication, responsive design, and engineering-focused project case studies.

## Website Overview

The portfolio is organized into five main areas:

### Home

The homepage provides a concise introduction to my background and current areas of work, with links to projects, technical writing, and other parts of the portfolio.

Recent blog posts are loaded from the blog metadata so the latest content can be surfaced on the homepage without manually updating every card.

### About

The About page presents my professional background, experience, technical skills, research interests, and career path across:

- Embedded computer vision
- Production computer vision
- Edge AI
- Applied AI
- Explainable AI
- Industrial AI systems

My work has progressed from resource-constrained embedded platforms to GPU-accelerated edge devices and multi-camera server systems.

### Projects

The Projects section focuses on the engineering work behind the systems rather than only presenting final results.

A hardware deployment path summarizes experience across different computing environments:

**STM32 → Raspberry Pi → NVIDIA Jetson → GPU Server**

Projects are organized into areas such as:

- **Computer Vision**
- **Explainable AI**
- **Additional Projects**

Selected projects include more detailed case studies describing the engineering process, system architecture, constraints, implementation decisions, optimization work, and lessons learned.

Examples include work on:

- Embedded fingerprint recognition
- Edge computer vision systems
- Multi-camera smart-city vision
- Real-time detection and tracking
- Industrial monitoring
- Explainable AI
- Multimodal AI
- Federated learning on edge devices

### Blog

The Blog is a collection of practical notes accumulated from development, research, deployment, and everyday engineering work.

Topics include areas such as:

- Git
- Docker
- DVC
- Python environments
- Pyenv
- UV
- Ubuntu
- Linux system files
- PATH and environment configuration
- Computer vision
- AI engineering

The articles are written primarily as practical references rather than complete tutorials.

Blog metadata is maintained separately so posts can be sorted and reused across different parts of the website.

### Life & Events

The Life & Events page records selected experiences outside the main project portfolio through a visual timeline.

It includes:

- Conferences
- Workshops
- Presentations
- Research events
- Professional activities
- Solo travel and personal journeys

The purpose of this section is to provide some context around the experiences accompanying my technical and professional development.

---

## Technical Focus

The portfolio reflects work across the full path from algorithms to deployed systems.

### Computer Vision

- Object detection
- Object tracking
- Image classification
- Semantic segmentation
- Face recognition
- License plate recognition
- Image processing
- Multi-camera systems

### Edge & Embedded AI

- STM32
- Raspberry Pi
- NVIDIA Jetson
- TensorRT
- ONNX
- TFLite
- Quantization
- Memory optimization
- Real-time inference

### AI & Deep Learning

- PyTorch
- TensorFlow
- Multitask learning
- Multimodal AI
- Federated learning
- Explainable AI
- Model optimization

### Engineering & Deployment

- Python
- C / C++
- OpenCV
- Linux
- Git
- Docker
- DVC
- MQTT
- PostgreSQL
- Grafana

---

## Repository Structure

A simplified view of the repository:

```text
.
├── index.html
├── about.html
├── project.html
├── blog.html
├── life_and_events.html
│
├── blog/
│   ├── development/
│   ├── ubuntu/
│   └── ...
│
├── projects/
│   └── ...
│
├── media/
│   ├── profile/
│   ├── projects/
│   ├── events/
│   └── ...
│
├── posts.json
└── README.md
```

The exact structure may continue to evolve as new projects and articles are added.

---

## Design Principles

The site is intentionally kept relatively simple.

The main goals are:

- **Content first** — technical content should remain the main focus.
- **Readable engineering documentation** — project pages should explain problems, decisions, trade-offs, and results.
- **Consistent structure** — common navigation, typography, spacing, comments, and section organization are used throughout the site.
- **Responsive layout** — pages adapt to desktop, tablet, and mobile screens.
- **Minimal dependencies** — the website does not require a large frontend framework.
- **Easy maintenance** — projects, articles, images, and events can be added directly to the repository.

---

## Running Locally

Because this is a static website, no build system is required.

Clone the repository:

```bash
git clone <repository-url>
cd <repository-name>
```

Then serve the directory using a local HTTP server.

For example, with Python:

```bash
python -m http.server 8000
```

Open:

```text
http://localhost:8000
```

A local server is recommended instead of opening `index.html` directly with `file://`, especially for features that load files such as JSON using JavaScript.

VS Code extensions such as **Live Server** can also be used.

---

## Adding Blog Content

Blog articles are stored as individual HTML pages.

When adding a new article:

1. Create the article in the appropriate blog subfolder.
2. Follow the existing article layout and code organization.
3. Add the corresponding metadata to `posts.json`.
4. Add any required images under `media/`.
5. Verify relative paths based on the article's folder depth.
6. Test the page using a local web server.
7. Check the layout on both desktop and mobile screen sizes.

Keeping the metadata updated allows recent articles to be reused automatically elsewhere on the site.

---

## Adding a Project

For a new project:

1. Add the project to the appropriate category in `project.html`.
2. Add its images and other media under `media/projects/`.
3. Create a dedicated project page when the project requires a deeper case study.
4. Describe the engineering problem, constraints, implementation, optimization process, and results rather than only listing technologies.
5. Link the project card to the case study.

The project section is intended to document **how systems were engineered**, including unsuccessful approaches, constraints, trade-offs, and iterative improvements where they are relevant.

---

## Development Notes

The project intentionally uses mostly native web technologies:

```text
HTML
CSS
JavaScript
JSON
```

JavaScript is used only where interaction or dynamic behavior is useful, such as:

- Project filtering
- Loading recent blog metadata
- Dynamic year information
- Small interface interactions

Most page content remains accessible directly from the HTML.

---

## Responsive Design

The website includes responsive layouts for different screen sizes.

Typical adaptations include:

- Multi-column layouts collapsing to a single column
- Project grids reducing the number of columns
- Hardware deployment paths changing from horizontal to vertical
- Navigation adapting to smaller screens
- Article tables of contents moving from sidebars into the normal page flow
- Images resizing while preserving their intended aspect ratio

---

## Project Status

This website is an ongoing personal project.

Content, project case studies, technical notes, images, and layout details are continuously refined as new work is added and older material is reorganized.

---

## Contact

**Duc An Nguyen**

Computer Vision / AI Engineer

- GitHub: [github.com/duc-an-nguyen](https://github.com/duc-an-nguyen)
- LinkedIn: [linkedin.com/in/ducannguyen](https://www.linkedin.com/in/ducannguyen)
- Email: [ducannguyen.da@gmail.com](mailto:ducannguyen.da@gmail.com)

---

© Duc An Nguyen