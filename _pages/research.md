---
permalink: /research/
title: "Research"
author_profile: true
redirect_from:
  - /wordpress/research/
---

<style>
  .research-page {
    --rp-ink: #172436;
    --rp-muted: #5d6878;
    --rp-blue: #075985;
    --rp-blue-dark: #0c3f5d;
    --rp-cyan: #0e7490;
    --rp-line: #d8e3ea;
    --rp-soft: #f4f8fb;
    --rp-white: #ffffff;
    color: var(--rp-ink);
    font-size: 1rem;
    line-height: 1.72;
  }

  .research-page *,
  .research-page *::before,
  .research-page *::after { box-sizing: border-box; }

  .research-page a { color: var(--rp-blue); }
  .research-page a:focus-visible {
    outline: 3px solid rgba(14, 116, 144, 0.3);
    outline-offset: 3px;
  }

  .rp-intro {
    position: relative;
    overflow: hidden;
    margin: 0 0 2rem;
    padding: clamp(1.4rem, 4vw, 2.7rem);
    color: var(--rp-white);
    background:
      radial-gradient(circle at 92% 18%, rgba(34, 211, 238, 0.22), transparent 27%),
      linear-gradient(135deg, #0b3148 0%, #075985 58%, #0e7490 100%);
    border-radius: 1.15rem;
    box-shadow: 0 18px 42px rgba(12, 63, 93, 0.18);
  }

  .rp-eyebrow {
    margin: 0 0 0.65rem;
    color: #b9edf5;
    font-size: 0.78rem;
    font-weight: 800;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }

  .rp-intro h2 {
    max-width: 760px;
    margin: 0;
    color: var(--rp-white);
    font-size: clamp(1.75rem, 4vw, 3rem);
    line-height: 1.12;
  }

  .rp-intro p {
    max-width: 760px;
    margin: 1rem 0 0;
    color: #e7f6fa;
    font-size: 1.06rem;
  }

  .rp-actions { display: flex; flex-wrap: wrap; gap: 0.7rem; margin-top: 1.35rem; }
  .rp-button {
    display: inline-flex;
    align-items: center;
    min-height: 44px;
    padding: 0.62rem 0.95rem;
    border: 1px solid rgba(255, 255, 255, 0.48);
    border-radius: 999px;
    color: var(--rp-white) !important;
    font-size: 0.9rem;
    font-weight: 750;
    text-decoration: none !important;
    transition: transform 160ms ease, background-color 160ms ease;
  }
  .rp-button:hover { transform: translateY(-1px); background: rgba(255,255,255,0.12); }
  .rp-button--solid { color: var(--rp-blue-dark) !important; background: var(--rp-white); border-color: var(--rp-white); }

  .rp-section-nav {
    display: grid;
    grid-template-columns: repeat(4, minmax(0, 1fr));
    gap: 0.8rem;
    margin: 0 0 2.8rem;
  }

  .rp-section-nav a {
    display: flex;
    min-height: 108px;
    padding: 1rem;
    flex-direction: column;
    justify-content: space-between;
    color: var(--rp-ink);
    background: var(--rp-white);
    border: 1px solid var(--rp-line);
    border-radius: 0.9rem;
    text-decoration: none !important;
    box-shadow: 0 7px 22px rgba(23, 36, 54, 0.06);
    transition: border-color 160ms ease, transform 160ms ease, box-shadow 160ms ease;
  }
  .rp-section-nav a:hover {
    transform: translateY(-2px);
    border-color: #8bbccc;
    box-shadow: 0 12px 26px rgba(23, 36, 54, 0.1);
  }
  .rp-section-nav span { color: var(--rp-cyan); font-size: 0.78rem; font-weight: 800; letter-spacing: 0.08em; }
  .rp-section-nav strong { display: block; margin-top: 0.7rem; font-size: 0.98rem; line-height: 1.35; }

  .rp-area {
    scroll-margin-top: 5rem;
    margin: 0 0 3.3rem;
    padding-top: 0.4rem;
  }
  .rp-area-header {
    display: grid;
    grid-template-columns: 68px minmax(0, 1fr);
    gap: 1rem;
    align-items: start;
    margin-bottom: 1.2rem;
  }
  .rp-area-number {
    display: grid;
    width: 58px;
    height: 58px;
    place-items: center;
    color: var(--rp-white);
    background: var(--rp-blue);
    border-radius: 50%;
    font-size: 1rem;
    font-weight: 850;
  }
  .rp-area h2 { margin: 0 0 0.4rem; color: var(--rp-ink); font-size: clamp(1.45rem, 3vw, 2rem); line-height: 1.2; }
  .rp-area-header p { max-width: 780px; margin: 0; color: var(--rp-muted); }

  .rp-feature {
    display: grid;
    grid-template-columns: minmax(0, 1.1fr) minmax(250px, 0.9fr);
    gap: 1.4rem;
    align-items: center;
    margin: 1.2rem 0;
    padding: 1.2rem;
    background: var(--rp-soft);
    border: 1px solid var(--rp-line);
    border-radius: 1rem;
  }
  .rp-feature img {
    width: 100%;
    max-height: 300px;
    object-fit: contain;
    padding: 0.55rem;
    background: var(--rp-white);
    border: 1px solid #e4edf2;
    border-radius: 0.75rem;
  }
  .rp-feature h3 { margin: 0 0 0.55rem; color: var(--rp-blue-dark); font-size: 1.18rem; }
  .rp-feature p { margin: 0; color: var(--rp-muted); }

  .rp-topic-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 0.85rem;
    margin-top: 1rem;
  }
  .rp-topic {
    padding: 1rem 1.05rem;
    background: var(--rp-white);
    border: 1px solid var(--rp-line);
    border-top: 3px solid #6ca9bc;
    border-radius: 0.75rem;
  }
  .rp-topic h3 { margin: 0 0 0.45rem; color: var(--rp-ink); font-size: 1.02rem; }
  .rp-topic p { margin: 0; color: var(--rp-muted); font-size: 0.94rem; }
  .rp-works { margin: 0.65rem 0 0; color: var(--rp-blue-dark); font-size: 0.86rem; font-weight: 700; }

  .rp-methods {
    margin: 3.2rem 0;
    padding: 1.35rem;
    background: #102f43;
    border-radius: 1rem;
    color: #e6f4f8;
  }
  .rp-methods h2 { margin: 0 0 0.9rem; color: var(--rp-white); font-size: 1.35rem; }
  .rp-method-list { display: flex; flex-wrap: wrap; gap: 0.55rem; }
  .rp-method-list span {
    padding: 0.45rem 0.7rem;
    background: rgba(255,255,255,0.08);
    border: 1px solid rgba(255,255,255,0.2);
    border-radius: 999px;
    font-size: 0.84rem;
  }

  .rp-current {
    margin: 3rem 0 1.6rem;
    padding: 1.35rem;
    border-left: 5px solid var(--rp-cyan);
    background: linear-gradient(90deg, #eef8fa, #f8fbfc);
    border-radius: 0 0.85rem 0.85rem 0;
  }
  .rp-current h2 { margin: 0 0 0.55rem; color: var(--rp-blue-dark); font-size: 1.35rem; }
  .rp-current p { margin: 0; color: var(--rp-muted); }

  .rp-footer-links {
    display: flex;
    flex-wrap: wrap;
    gap: 0.8rem;
    align-items: center;
    padding: 1.2rem 0 0.4rem;
    border-top: 1px solid var(--rp-line);
  }
  .rp-footer-links a { font-weight: 750; text-decoration-thickness: 1px; text-underline-offset: 3px; }

  @media (max-width: 820px) {
    .rp-section-nav { grid-template-columns: repeat(2, minmax(0, 1fr)); }
    .rp-feature { grid-template-columns: 1fr; }
  }

  @media (max-width: 560px) {
    .rp-intro { border-radius: 0.8rem; }
    .rp-section-nav, .rp-topic-grid { grid-template-columns: 1fr; }
    .rp-section-nav a { min-height: 88px; }
    .rp-area-header { grid-template-columns: 48px minmax(0, 1fr); gap: 0.75rem; }
    .rp-area-number { width: 44px; height: 44px; }
  }

  @media (prefers-reduced-motion: reduce) {
    .rp-button, .rp-section-nav a { transition: none; }
  }
</style>

<main class="research-page">
  <section class="rp-intro" aria-labelledby="research-intro-title">
    <p class="rp-eyebrow">Cyber-physical systems · Smart cities · Machine learning · Control</p>
    <h2 id="research-intro-title">Human-centered intelligence for urban systems</h2>
    <p>My group studies how people, physical infrastructure, and data interact. We develop sensing, learning, optimization, and control methods for reliable urban services, electric mobility, energy systems, edge intelligence, and smart infrastructure.</p>
    <div class="rp-actions">
      <a class="rp-button rp-button--solid" href="{{ '/publications/' | relative_url }}">View publications</a>
      <a class="rp-button" href="https://scholar.google.com/citations?user=mGnjOOUAAAAJ&amp;hl=en" target="_blank" rel="noopener">Google Scholar</a>
    </div>
  </section>

  <nav class="rp-section-nav" aria-label="Research areas">
    <a href="#mobility-energy"><span>AREA 01</span><strong>Smart Mobility and Energy Systems</strong></a>
    <a href="#urban-services"><span>AREA 02</span><strong>Human-Centered Urban Cyber-Physical Systems</strong></a>
    <a href="#edge-systems"><span>AREA 03</span><strong>Edge Intelligence and Networked Systems</strong></a>
    <a href="#sensing-buildings"><span>AREA 04</span><strong>Intelligent Sensing and Built Environments</strong></a>
  </nav>

  <section class="rp-area" id="mobility-energy" aria-labelledby="mobility-energy-title">
    <header class="rp-area-header">
      <div class="rp-area-number" aria-hidden="true">01</div>
      <div>
        <h2 id="mobility-energy-title">Smart Mobility and Energy Systems</h2>
        <p>Electric transportation connects mobility demand, charging infrastructure, renewable energy, and the power grid. We coordinate these systems while maintaining transportation service quality.</p>
      </div>
    </header>

    <div class="rp-feature">
      <div>
        <h3>Electric taxi charging and grid coordination</h3>
        <p>We design real-time methods for charging and dispatch, renewable-energy use, power-system limits, fairness during failures, and fleet participation in demand response.</p>
        <p class="rp-works">Representative systems: p²Charging · SAC · SOURCE · POET · eFlx</p>
      </div>
      <img src="{{ '/images/p2charging.png' | relative_url }}" alt="Electric taxi charging and dispatch coordination framework" loading="lazy">
    </div>

    <div class="rp-topic-grid">
      <article class="rp-topic">
        <h3>Energy flexibility and demand response</h3>
        <p>We model and prepare the charging flexibility of electric fleets so they can respond to grid requests without reducing passenger service.</p>
        <p class="rp-works">ICCPS 2025 · ACM TCPS 2025</p>
      </article>
      <article class="rp-topic">
        <h3>Shared electric micromobility</h3>
        <p>We study charging, rebalancing, human preferences, and regulation for shared electric bicycles and scooters operated by one or more companies.</p>
        <p class="rp-works">CIKM 2023 · ICRA 2024 · SIGSPATIAL 2025</p>
      </article>
      <article class="rp-topic">
        <h3>Mobility under power disruptions</h3>
        <p>We coordinate limited charging power and vehicle service during shortages and failures, with attention to service loss and regional fairness.</p>
        <p class="rp-works">ACC 2024 · ACC 2025</p>
      </article>
      <article class="rp-topic">
        <h3>Multi-modal transportation</h3>
        <p>We integrate transportation modes when disruptions change passenger flows and reduce the capacity of part of the network.</p>
        <p class="rp-works">ICCPS 2018 · IEEE TMC 2023</p>
      </article>
    </div>
  </section>

  <section class="rp-area" id="urban-services" aria-labelledby="urban-services-title">
    <header class="rp-area-header">
      <div class="rp-area-number" aria-hidden="true">02</div>
      <div>
        <h2 id="urban-services-title">Human-Centered Urban Cyber-Physical Systems</h2>
        <p>Urban services depend on residents, public agencies, physical resources, and automated decisions. We study incomplete reports, changing service requirements, resource allocation, and feedback between people and service systems.</p>
      </div>
    </header>

    <div class="rp-feature">
      <div>
        <h3>Municipal service intelligence and coordination</h3>
        <p>We use municipal 311 data to estimate demand and service time, then connect these estimates to resource decisions. We also study how city services can negotiate when they compete for limited resources.</p>
        <p class="rp-works">Representative systems: MuST²-Learn · DeResolver</p>
      </div>
      <img src="{{ '/images/deresolver%20figure.png' | relative_url }}" alt="Decentralized service coordination framework" loading="lazy">
    </div>

    <div class="rp-topic-grid">
      <article class="rp-topic">
        <h3>Municipal 311 analytics</h3>
        <p>We model sparse and heterogeneous service requests across locations, request types, and time to estimate future demand and completion time.</p>
        <p class="rp-works">SIGSPATIAL 2025 · Ongoing research</p>
      </article>
      <article class="rp-topic">
        <h3>Multi-service conflict resolution</h3>
        <p>DeResolver lets urban services exchange proposals and reach resource-sharing decisions through decentralized negotiation.</p>
        <p class="rp-works">ICCPS 2021 Best Paper · ACM TCPS 2022</p>
      </article>
      <article class="rp-topic">
        <h3>Human-generated sensing</h3>
        <p>We study how selective, delayed, repeated, and incomplete reports affect estimates of public needs and later service decisions.</p>
        <p class="rp-works">Current direction</p>
      </article>
      <article class="rp-topic">
        <h3>Human-system feedback</h3>
        <p>We examine how service outcomes change future reporting and how explanations can support accountable closed-loop decisions.</p>
        <p class="rp-works">Current direction</p>
      </article>
    </div>
  </section>

  <section class="rp-area" id="edge-systems" aria-labelledby="edge-systems-title">
    <header class="rp-area-header">
      <div class="rp-area-number" aria-hidden="true">03</div>
      <div>
        <h2 id="edge-systems-title">Edge Intelligence and Networked Systems</h2>
        <p>Edge intelligence places learning and computing close to mobile users and physical systems. We coordinate models, computation, services, and communication across heterogeneous devices.</p>
      </div>
    </header>

    <div class="rp-topic-grid">
      <article class="rp-topic">
        <h3>Federated intelligence deployment</h3>
        <p>We use similarity-aware aggregation and semi-asynchronous learning to speed the deployment of federated models across heterogeneous edge systems.</p>
        <p class="rp-works">INFOCOM 2025</p>
      </article>
      <article class="rp-topic">
        <h3>Service migration for edge learning</h3>
        <p>We coordinate migration and reuse of learning services across mobile edge nodes with different data modalities and computing resources.</p>
        <p class="rp-works">MobiHoc 2023</p>
      </article>
      <article class="rp-topic">
        <h3>Information-centric edge networking</h3>
        <p>We connect information-centric networking with reinforcement learning and transport design in mobile edge environments.</p>
        <p class="rp-works">MASS 2024 · IWQoS 2024</p>
      </article>
      <article class="rp-topic">
        <h3>Computing-service placement</h3>
        <p>We place service-function chains across heterogeneous edge devices while accounting for delay, hardware, and resource limits.</p>
        <p class="rp-works">IEEE Transactions on Computers 2024</p>
      </article>
    </div>
  </section>

  <section class="rp-area" id="sensing-buildings" aria-labelledby="sensing-buildings-title">
    <header class="rp-area-header">
      <div class="rp-area-number" aria-hidden="true">04</div>
      <div>
        <h2 id="sensing-buildings-title">Intelligent Sensing and Built Environments</h2>
        <p>We combine sensing, prediction, and control to understand people and physical spaces, improve building operation, and study the privacy and security of contactless sensing.</p>
      </div>
    </header>

    <div class="rp-feature">
      <div>
        <h3>Occupancy-aware building control</h3>
        <p>We extract fine-grained occupancy patterns and use them in HVAC control. Current work also studies indoor environmental quality through connected sensing and data-driven control.</p>
        <p class="rp-works">IoTDI 2020 · Current school-building research</p>
      </div>
      <img src="{{ '/images/hvaccontrol.png' | relative_url }}" alt="Occupancy-aware building control framework" loading="lazy">
    </div>

    <div class="rp-topic-grid">
      <article class="rp-topic">
        <h3>Contactless human sensing</h3>
        <p>We investigate mmWave sensing for speaker analysis and remote observation, together with the security and privacy risks created by these capabilities.</p>
        <p class="rp-works">SenSys 2025 · INFOCOM 2026</p>
      </article>
      <article class="rp-topic">
        <h3>Indoor environmental quality</h3>
        <p>We study sensing and control of particulate matter, carbon dioxide, temperature, humidity, and ventilation in occupied buildings.</p>
        <p class="rp-works">Current direction</p>
      </article>
    </div>
  </section>

  <section class="rp-methods" aria-labelledby="methods-title">
    <h2 id="methods-title">Methods across research areas</h2>
    <div class="rp-method-list">
      <span>Optimization and model predictive control</span>
      <span>Reinforcement learning</span>
      <span>Game theory and multi-agent systems</span>
      <span>Spatial-temporal learning</span>
      <span>Federated and edge learning</span>
      <span>Wireless and mmWave sensing</span>
      <span>Data-driven system evaluation</span>
    </div>
  </section>

  <section class="rp-current" aria-labelledby="current-title">
    <h2 id="current-title">Current directions</h2>
    <p>Current projects study human-aligned urban services, edge-assisted autonomous transportation, indoor environmental sensing, and cascading disruptions across transportation and power networks.</p>
  </section>

  <footer class="rp-footer-links" aria-label="Research links">
    <a href="{{ '/publications/' | relative_url }}">All publications</a>
    <span aria-hidden="true">·</span>
    <a href="https://scholar.google.com/citations?user=mGnjOOUAAAAJ&amp;hl=en" target="_blank" rel="noopener">Google Scholar</a>
    <span aria-hidden="true">·</span>
    <a href="mailto:yukun-yuan@utc.edu">Research collaboration</a>
  </footer>
</main>
