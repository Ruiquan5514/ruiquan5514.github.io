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
    padding: 1.5rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 0.5rem;
    background: var(--global-card-bg-color);
  }
  .course-resources .course-demo h3 {
    margin-bottom: 1rem;
    font-size: 1.4rem;
  }
  .course-resources .course-demo ul {
    padding-left: 1.25rem;
  }
  .course-resources .course-demo li + li {
    margin-top: 0.5rem;
  }
  .course-resources .course-demo-link {
    display: inline-block;
    padding: 0.65rem 0.9rem;
    border: 1px solid currentColor;
    border-radius: 0.3rem;
    font-weight: 500;
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
  <p>Watch the lecture and explore reinforcement learning through interactive demonstrations.</p>

  <nav class="course-navigation" aria-label="Course resources">
    <a href="#lecture-video">Watch the lecture</a>
    <a href="#visualizations">Explore the algorithms</a>
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
    <h2 id="visualizations-title">Interactive algorithm visualizations</h2>
    <p>Compare how policies learn from experience, or follow a tree search before choosing a move.</p>

    <div class="course-demo-grid">
      <article class="course-demo" aria-labelledby="policy-title">
        <h3 id="policy-title">Policy gradients and actor–critic</h3>
        <p>
          Replay REINFORCE, one-step actor–critic, and PPO-Clip in the same Gridworld. Track episodic returns,
          agent trajectories, and estimated state values over 220 training episodes.
        </p>
        <p><a class="course-demo-link" href="https://ruiquan5514.github.io/CS667-585-RL/">Compare the algorithms</a></p>
        <p>Jump to an algorithm in the shared replay:</p>
        <ul>
          <li><a href="https://ruiquan5514.github.io/CS667-585-RL/#reinforce-view">REINFORCE + baseline</a> — updates after each episode.</li>
          <li><a href="https://ruiquan5514.github.io/CS667-585-RL/#actor-critic-view">One-step actor–critic</a> — updates after each transition.</li>
          <li><a href="https://ruiquan5514.github.io/CS667-585-RL/#ppo-view">PPO-Clip</a> — clipped updates after each rollout batch.</li>
        </ul>
        <p>Select one or more algorithms in the demo, then play, pause, or scrub the training timeline.</p>
      </article>

      <article class="course-demo" aria-labelledby="mcts-title">
        <h3 id="mcts-title">Monte Carlo Tree Search / UCT</h3>
        <p>
          Explore planning in tic-tac-toe. Edit a board position, choose a fixed opponent policy, and inspect
          how UCT builds a search tree before the agent makes a move.
        </p>
        <p><a class="course-demo-link" href="https://ruiquan5514.github.io/CS667-585-RL/mcts/">Explore MCTS / UCT</a></p>
        <ul>
          <li>Run one simulation or complete a 512-simulation search.</li>
          <li>Inspect the selected path, new nodes, and root-action visit counts.</li>
          <li>Undo a simulation, or pan and zoom through the full tree.</li>
        </ul>
        <p>After searching, make the selected move to see the resulting game position.</p>
      </article>
    </div>

  </section>
</div>
