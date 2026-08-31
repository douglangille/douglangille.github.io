---
layout: none
permalink: /hub/
---
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Doug Langille</title>
<style>
  :root {
    --bg: #1a1a1e;
    --card-bg: #232328;
    --text: #e8e6e1;
    --muted: #9a978f;
    --accent: #d4a017; /* warm amber — not blue (digital) or black/red (fiction) */
    --digital-color: #3a7ca5;
    --fiction-color: #6b2d3c;
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body {
    background: var(--bg);
    color: var(--text);
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 2rem 1rem;
  }
  .wrap {
    max-width: 640px;
    width: 100%;
  }
  h1 {
    font-size: 1.6rem;
    font-weight: 600;
    margin-bottom: 0.4rem;
  }
  .tagline {
    color: var(--muted);
    font-size: 1rem;
    margin-bottom: 2rem;
    line-height: 1.5;
  }
  .blocks {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1rem;
    margin-bottom: 2rem;
  }
  @media (max-width: 480px) {
    .blocks { grid-template-columns: 1fr; }
  }
  .block {
    display: block;
    background: var(--card-bg);
    border-radius: 10px;
    padding: 1.4rem;
    text-decoration: none;
    color: var(--text);
    border-left: 4px solid transparent;
    transition: transform 0.15s ease, border-color 0.15s ease;
  }
  .block:hover {
    transform: translateY(-2px);
  }
  .block.digital {
    border-left-color: var(--digital-color);
  }
  .block.fiction {
    border-left-color: var(--fiction-color);
  }
  .block-label {
    font-size: 0.7rem;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    color: var(--muted);
    margin-bottom: 0.3rem;
  }
  .block-title {
    font-size: 1.15rem;
    font-weight: 600;
    margin-bottom: 0.3rem;
  }
  .block-desc {
    font-size: 0.85rem;
    color: var(--muted);
    line-height: 1.4;
  }
  .contact {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    font-size: 0.9rem;
    border-top: 1px solid #333;
    padding-top: 1.2rem;
  }
  .contact a {
    color: var(--accent);
    text-decoration: none;
  }
  .contact a:hover {
    text-decoration: underline;
  }
</style>
</head>
<body>
  <div class="wrap">
    <h1>Doug Langille</h1>
    <p class="tagline">26 years in IT leadership and edtech at NSCC. On the side, I write about digital strategy and dark fiction — different voices, same person.</p>

    <div class="blocks">
      <a class="block digital" href="https://digital.douglangille.ca">
        <div class="block-label">Nonfiction</div>
        <div class="block-title">Digital Doug</div>
        <div class="block-desc">Weekly writing on AI, edtech, and digital strategy.</div>
      </a>
      <a class="block fiction" href="https://douglangille.ca">
        <div class="block-label">Fiction</div>
        <div class="block-title">Darkling Whim</div>
        <div class="block-desc">Flash fiction in the Thoughtful Magic universe.</div>
      </a>
    </div>

    <div class="contact">
      <a href="mailto:me@douglangille.ca">Email</a>
      <a href="[LINKEDIN_URL]">LinkedIn</a>
      <a href="[AMAZON_AUTHOR_URL]">Amazon Author Page</a>
      <!-- add more social links here as needed, same pattern -->
    </div>
  </div>
</body>
</html>
