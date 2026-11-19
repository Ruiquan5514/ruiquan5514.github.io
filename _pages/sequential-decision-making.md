---
layout: page
title: Sequential Decision Making
permalink: /teaching/sequential-decision-making/
description: CS 667/585 · University of Kentucky · Fall 2026
nav: false
_styles: |
  .course-resources section {
    margin-top: 2.5rem;
    scroll-margin-top: 6rem;
  }
  .course-resources .course-navigation {
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem 1.5rem;
    margin: 1.5rem 0;
  }
  .course-resources .course-video {
    position: relative;
    aspect-ratio: 16 / 9;
    overflow: hidden;
    border: 1px solid var(--global-divider-color);
    border-radius: 0.5rem;
    background: #000;
  }
  .course-resources .course-video iframe {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    border: 0;
  }
  .course-resources .course-video-link {
    margin-top: 0.75rem;
  }
  .course-resources .course-demo-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1.25rem;
    margin-top: 1.5rem;
  }
  .course-resources .course-demo {
    display: block;
    padding: 1.5rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 0.5rem;
    background: var(--global-card-bg-color);
  }
  .course-resources .course-demo h3 {
    margin: 0;
    font-size: 1.4rem;
  }
  .course-resources a:focus-visible {
    outline: 2px solid var(--global-theme-color);
    outline-offset: 4px;
  }
  @media (max-width: 700px) {
    .course-resources .course-demo-grid {
      grid-template-columns: 1fr;
    }
  }
---

<div class="course-resources">
  <p><a href="/teaching/">All courses</a></p>

  <nav class="course-navigation" aria-label="Course resources">
    <a href="#lecture-video">Video</a>
    <a href="#visualizations">Interactive visualizations</a>
  </nav>

  <section id="lecture-video" aria-labelledby="lecture-title">
    <h2 id="lecture-title">RL in the wild</h2>
    <div class="course-video">
      <iframe
        src="https://www.youtube-nocookie.com/embed/aL9yREqsO20"
        title="RL in the wild — Ruiquan Huang"
        width="960"
        height="540"
        loading="lazy"
        allow="accelerometer; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        referrerpolicy="strict-origin-when-cross-origin"
        allowfullscreen
      ></iframe>
    </div>
    <p class="course-video-link"><a href="https://www.youtube.com/watch?v=aL9yREqsO20">Watch on YouTube</a></p>
  </section>

  <section id="visualizations" aria-labelledby="visualizations-title">
    <h2 id="visualizations-title">Interactive visualizations</h2>

    <div class="course-demo-grid">
      <a class="course-demo" href="https://ruiquan5514.github.io/CS667-585-RL/">
        <h3>Policy Gradient</h3>
      </a>
      <a class="course-demo" href="https://ruiquan5514.github.io/CS667-585-RL/mcts/">
        <h3>Tree Search (MCTS / UCT)</h3>
      </a>
    </div>

  </section>
</div>
