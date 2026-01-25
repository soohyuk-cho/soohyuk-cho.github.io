---
layout: page
permalink: /coursework/
title: Coursework
description: Here's a full listing of technical classes I've taken.
nav: true
nav_order: 2
---

<!-- ===== School Toggle ===== -->
<div class="school-wrapper">

  <!-- Radios first so we can target content with CSS (no JS required) -->
  <input type="radio" name="school" id="opt-princeton" class="sr-only">
  <input type="radio" name="school" id="opt-berkeley" class="sr-only" checked>

  <!-- Segmented control -->
  <div class="segmented" role="tablist" aria-label="Select school">
    <label for="opt-princeton" role="tab" aria-controls="princeton" tabindex="0">Princeton</label>
    <label for="opt-berkeley" role="tab" aria-controls="berkeley" tabindex="0">Berkeley</label>
  </div>

  <!-- Content panes -->
  <div class="school-content">

    <!-- Princeton -->
    <section id="princeton" data-school="princeton" role="tabpanel" aria-labelledby="opt-princeton" markdown="1">

### Princeton Coursework
<details markdown="1">
  <summary><em>Fall 2025</em></summary>

- [COS 516/ECE 516: Automated Reasoning about Software](https://www.cs.princeton.edu/courses/archive/fall25/cos516/)
- [ECE 574: Security and Privacy in Computing and Communications](https://www.princeton.edu/~pmittal/teaching/ece574-fall25/index.html) (A+)
- ECE 580: Advanced Topics in Computer Engineering: Domain-specific Computer Systems Architecture
- ECE 518: Selected Topics in Computer Engineering and Information Sciences and Systems (Seminar)

</details>

<details markdown="1">
  <summary><em>Spring 2026</em></summary>

TBD

</details>

<!-- Example template:
<details markdown="1">
  <summary><em>Fall 2025</em></summary>

- ECE 5xx: (Course Title)
- COS 5xx: (Course Title)

</details>
-->

</section>

<!-- Berkeley -->
<section id="berkeley" data-school="berkeley" role="tabpanel" aria-labelledby="opt-berkeley" markdown="1">

### UC Berkeley Coursework
<details markdown="1">
  <summary><em>Spring 2025</em></summary>

- EE 194: 16nm SoC for IoT Tapeout
- [DATA C100: Principles & Techniques of Data Science](https://ds100.org/sp25/)
- [MATH 156: Numerical Analysis for Data Science and Statistics](https://classes.berkeley.edu/content/2025-spring-math-156-001-lec-001) (A+)

</details>

<details markdown="1">
  <summary><em>Fall 2024</em></summary>

- [CS 168: Introduction to the Internet: Architecture and Protocols](https://www2.eecs.berkeley.edu/Courses/CS168/)
- [CS 186: Introduction to Database Systems](https://www2.eecs.berkeley.edu/Courses/CS186/)
- [BIOENG 100: Ethics in Science and Engineering](https://classes.berkeley.edu/content/2024-fall-bioeng-100-001-lec-001)
- [CIVENG 153: Transportation Facility Design (Airport Design)](https://classes.berkeley.edu/content/2024-fall-civeng-153-001-lec-001)
</details>

<details markdown="1">
  <summary><em>Spring 2024</em></summary>

- [CS 164: Programming Languages and Compilers](https://sites.google.com/berkeley.edu/cs164sp24/home)  
- EE 105: Microelectronic Devices and Circuits  
- EECS 151: Introduction to Digital Design and Integrated Circuits  
- EECS 151LB: Field-Programmable Gate Array Laboratory (FPGA)  
- [EECS C106B: Robotic Manipulation and Interaction](https://ucb-ee106.github.io/106b-sp24site/)

</details>

<details markdown="1">
  <summary><em>Fall 2023</em></summary>

- [CS 162: Operating Systems and System Programming](https://inst.eecs.berkeley.edu/~cs162/fa23/)  
- [EECS C106A: Introduction to Robotics](https://ucb-ee106.github.io/eecs106a-fa23site/)  
- [CS 285: (Grad) Deep Reinforcement Learning, Decision Making, and Control](https://rail.eecs.berkeley.edu/deeprlcourse/)  
- EE 221A: (Grad) Linear System Theory

</details>

<details markdown="1">
  <summary><em>Spring 2023</em></summary>

- [CS 152: Computer Architecture and Engineering](https://inst.eecs.berkeley.edu/~cs152/sp23/)  
- [CS 189: Introduction to Machine Learning](https://people.eecs.berkeley.edu/~jrs/189s23/) (A+)  
- [EECS 127: Optimization Models in Engineering](https://inst.eecs.berkeley.edu/~eecs127/sp23/)

</details>

<details markdown="1">
  <summary><em>Fall 2022</em></summary>

- [CS 61C: Computer Architecture and Engineering](https://inst.eecs.berkeley.edu/~cs61c/fa22/)  
- [CS 170: Efficient Algorithms and Intractable Problems](https://cs170.org/)  
- [EECS 126: Probability and Random Processes](https://inst.eecs.berkeley.edu/~ee126/fa22/)  
- EE 120: Signals and Systems

</details>

<details markdown="1">
  <summary><em>Spring 2021</em></summary>

- [CS 61B: Data Structures](https://sp21.datastructur.es/) (A+)  
- [CS 70: Discrete Mathematics and Probability Theory](https://www.sp21.eecs70.org/)  
- [EECS 16B: Designing Information Devices and Systems II](https://inst.eecs.berkeley.edu/~ee16b/sp21/)

</details>

<details markdown="1">
  <summary><em>Fall 2020</em></summary>

- [CS 61A: The Structure and Interpretation of Computer Programs](https://inst.eecs.berkeley.edu/~cs61a/fa20/) (A+)  
- [EECS 16A: Designing Information Devices and Systems I](https://inst.eecs.berkeley.edu/~ee16a/fa20/)  
- [Data C8: Foundations of Data Science](https://www.data8.org/fa20/)

</details>

> **Note:** *Fall 2021 & Spring 2022 — gap year for military service, Republic of Korea Army.*

</section>
</div>
</div>

<style>
/* ----------------------------
   Component-scoped color tokens
   ---------------------------- */
.school-wrapper {
  /* Light defaults */
  --seg-border: #d0d7de;
  --seg-bg: #f6f8fa;
  --seg-active-bg: #ffffff;
  --seg-shadow: 0 1px 2px rgba(0,0,0,0.06), 0 0 0 1px rgba(0,0,0,0.04) inset;
  --seg-focus: rgba(27,127,204,0.35);

  --text: #111827;
  --muted: #6b7280;
  --card-bg: #ffffff;
  --card-border: #e5e7eb;
}

/* System dark (only emit if site-wide dark mode is enabled) */
{% if site.enable_darkmode %}
@media (prefers-color-scheme: dark) {
  .school-wrapper {
    --seg-border: #3f3f46;
    --seg-bg: #111827;
    --seg-active-bg: #1f2937;
    --seg-shadow: 0 1px 2px rgba(0,0,0,0.4), 0 0 0 1px rgba(255,255,255,0.06) inset;
    --seg-focus: rgba(56,189,248,0.45);

    --text: #e5e7eb;
    --muted: #9ca3af;
    --card-bg: #111827;
    --card-border: #374151;
  }
}

/* Manual theme toggles (override system) */
html[data-theme="light"] .school-wrapper,
html.light .school-wrapper,
body.light .school-wrapper,
.theme-light .school-wrapper {
  --seg-border: #d0d7de;
  --seg-bg: #f6f8fa;
  --seg-active-bg: #ffffff;
  --seg-shadow: 0 1px 2px rgba(0,0,0,0.06), 0 0 0 1px rgba(0,0,0,0.04) inset;
  --seg-focus: rgba(27,127,204,0.35);
  --text: #111827;
  --muted: #6b7280;
  --card-bg: #ffffff;
  --card-border: #e5e7eb;
}

html[data-theme="dark"] .school-wrapper,
html[data-color-scheme="dark"] .school-wrapper,
html.dark .school-wrapper,
body.dark .school-wrapper,
.dark .school-wrapper,
.theme-dark .school-wrapper {
  --seg-border: #3f3f46;
  --seg-bg: #111827;
  --seg-active-bg: #1f2937;
  --seg-shadow: 0 1px 2px rgba(0,0,0,0.4), 0 0 0 1px rgba(255,255,255,0.06) inset;
  --seg-focus: rgba(56,189,248,0.45);
  --text: #e5e7eb;
  --muted: #9ca3af;
  --card-bg: #111827;
  --card-border: #374151;
}
{% endif %}

/* ----------------------------
   Component styles (use tokens)
   ---------------------------- */

/* Accessibility helper */
.school-wrapper .sr-only {
  position: absolute !important;
  width: 1px; height: 1px;
  padding: 0; margin: -1px;
  overflow: hidden; clip: rect(0,0,0,0);
  white-space: nowrap; border: 0;
}

/* Segmented control */
.school-wrapper .segmented {
  display: inline-flex;
  border: 1px solid var(--seg-border);
  border-radius: 9999px;
  padding: 4px;
  gap: 4px;
  background: var(--seg-bg);
  margin: 0 0 1rem 0;
}

.school-wrapper .segmented label {
  font: 500 0.95rem/1.2 system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji", "Segoe UI Emoji";
  color: var(--text);
  padding: 0.5rem 0.9rem;
  border-radius: 9999px;
  cursor: pointer;
  user-select: none;
  outline: none;
  transition: background 120ms ease, box-shadow 120ms ease;
}

.school-wrapper .segmented label:focus-visible {
  box-shadow: 0 0 0 3px var(--seg-focus);
}

.school-wrapper #opt-princeton:checked ~ .segmented label[for="opt-princeton"],
.school-wrapper #opt-berkeley:checked  ~ .segmented label[for="opt-berkeley"] {
  background: var(--seg-active-bg);
  box-shadow: var(--seg-shadow);
}

/* Content panes */
.school-wrapper .school-content [data-school] { display: none; }
.school-wrapper #opt-princeton:checked ~ .school-content [data-school="princeton"] { display: block; }
.school-wrapper #opt-berkeley:checked  ~ .school-content [data-school="berkeley"]  { display: block; }

/* Accordion */
.school-wrapper details {
  border: 1px solid var(--card-border);
  border-radius: 10px;
  padding: .5rem .9rem;
  margin: .5rem 0;
  background: var(--card-bg);
}

.school-wrapper details > summary {
  list-style: none;
  cursor: pointer;
  font-weight: 600;
  color: var(--text);
  display: flex;
  align-items: center;
  gap: .5rem;
}

.school-wrapper details > summary::-webkit-details-marker { display: none; }

.school-wrapper details > summary::before {
  content: "▸";
  display: inline-block;
  transform: translateY(-1px);
  transition: transform 120ms ease;
}

.school-wrapper details[open] > summary::before {
  transform: rotate(90deg) translateX(1px);
}

.school-wrapper details > *:not(summary) { margin-top: .6rem; }
</style>

<script>
/* Enhance a11y: keep aria-selected and hidden in sync for tabs */
document.addEventListener('DOMContentLoaded', () => {
  const inputs = {
    princeton: document.getElementById('opt-princeton'),
    berkeley: document.getElementById('opt-berkeley')
  };
  const labels = document.querySelectorAll('.segmented label');
  const panes = {
    princeton: document.querySelector('[data-school="princeton"]'),
    berkeley: document.querySelector('[data-school="berkeley"]')
  };

  function update() {
    const active = inputs.princeton.checked ? 'princeton' : 'berkeley';
    labels.forEach(l => l.setAttribute('aria-selected', (l.getAttribute('for') === 'opt-' + active) ? 'true' : 'false'));
    panes.princeton.hidden = active !== 'princeton';
    panes.berkeley.hidden = active !== 'berkeley';
  }

  Object.values(inputs).forEach(i => i.addEventListener('change', update));
  labels.forEach(l => {
    l.addEventListener('keydown', (e) => {
      if (e.key === 'Enter' || e.key === ' ') {
        e.preventDefault();
        const target = document.getElementById(l.getAttribute('for'));
        if (target) { target.checked = true; target.dispatchEvent(new Event('change')); }
      }
    });
  });

  update();
});
</script>
