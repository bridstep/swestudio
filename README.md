# swestudio.dev — Personal Portfolio & Web Hub

Welcome to the source repository for **swestudio.dev**, the personal portfolio and digital hub for **Stephen Bridges**.

This project was built from the ground up with a focus on clean semantic HTML, modern CSS architecture, and an interactive, spatial user interface—without relying on heavy front-end frameworks.

## 🎯 Project Overview & Design Philosophy

Rather than using a standard linear layout, `swestudio.dev` utilizes a **honeycomb grid navigation system** paired with a **3D glassmorphism (`glass3d`) aesthetic**.

* **Zero-Framework Performance:** Built purely with vanilla HTML5 and CSS3 to ensure near-instant load times, minimal overhead, and complete control over layout rendering and visual effects.

* **Spatial & Tactile UI:** Ambient background lighting (`.bg-glow`) works in tandem with backdrop filters and custom hexagonal geometry (`.hex-wrapper`) to create depth, saturation, and a modern, interactive feel.

* **Employer-Centric Navigation:** Designed as a central launchpad that gives recruiters and engineering managers immediate, one-click access to my resume, technical projects, professional background, and networking links.

## 🏗️ Architectural Decisions: Why a Static Site?

Choosing a pure static architecture for `swestudio.dev` was a deliberate decision driven by both infrastructure constraints and a desire to sharpen core web engineering fundamentals:

* **Working Within Infrastructure Constraints (Nginx):** The production server hosting this portfolio runs an Nginx instance strictly configured to serve static assets. Designing around this constraint required eliminating server-side runtime dependencies and optimizing static asset delivery—an exercise in pragmatic engineering and tailoring solutions to the target environment.
* **First-Principles Engineering:** Building complex layouts (like the responsive honeycomb grid) and visual effects (3D glassmorphism) without abstractions forces a deep understanding of the browser's rendering engine, the CSS box model, and native DOM behavior.
* **Appreciating Modern Frameworks:** Stripping away modern tooling highlights the exact problems that libraries and frameworks like React, Vue, or Tailwind CSS solve—such as component reusability, state synchronization, and scoped styling. Navigating those challenges manually in vanilla HTML/CSS provides a stronger foundation and deeper appreciation for when and why to adopt those tools in larger production applications.

## 🗂️ Site Architecture

The landing page (`index.html`) serves as the central hub, routing visitors to dedicated, single-purpose views:

* **`index.html`** — The primary honeycomb navigation hub featuring ambient glow effects and responsive hex rows.

* **`about.html`** — Professional background, engineering philosophy, and core competencies.

* **`projects.html`** — Technical case studies, architectural breakdowns, and live demos.

* **`resume.html`** — Web-formatted curriculum vitae and work history.

* **`contact.html`** — Direct communication channels and inquiry details.

* **`qr_code.html`** — Quick-scan mobile sharing utility for in-person networking and conferences.

* **`fun.html` (`***`)** — A dedicated space for creative coding experiments and interactive easter eggs.

## 🛠️ Technical Highlights

* **Semantic HTML5:** Structured using accessible landmarks (`<main>`) and clean, maintainable class naming conventions.

* **Custom Geometric Layouts:** Engineered multi-row hexagonal alignment (`.honeycomb-container` & `.hex-row`) using pure CSS positioning and flexbox/grid techniques.

* **Glassmorphism & Lighting:** Layered CSS blur, saturation, and ambient glow nodes (`glow-1`, `glow-2`) to achieve a frosted-glass effect that adapts dynamically to viewport dimensions.

* **Responsive Design:** Configured with viewport meta tags and scalable containers to maintain visual integrity across desktop monitors and mobile devices.

## 📁 Directory Structure

```
swestudio.dev/
├── index.html          # Main honeycomb landing page
├── about.html          # Biography & skills
├── projects.html       # Software engineering portfolio
├── resume.html         # Digital resume
├── contact.html        # Contact information
├── qr_code.html        # Networking QR code view
├── fun.html            # Experimental / interactive playground
├── styles/
│   └── index.css       # Core layout, hexagonal geometry, and glass3d styling
└── assets/
    └── fire.svg        # Custom vector favicon and branding assets

```
