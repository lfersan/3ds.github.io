<style>
:root {
  --primary: #ff6b6b;
  --secondary: #b8c1ec;
  --muted: #94a3b8;
  --card: rgba(255,255,255,0.04);
  --border: rgba(255,255,255,0.08);
  --bg: #080f1f;
  --panel: #111a2f;
  --panel-soft: #182441;
}
body {
  background: radial-gradient(circle at top, #101a32 0%, #080f1f 55%, #050914 100%);
  color: #e2e8f0;
  font-family: "Segoe UI", "Inter", system-ui, -apple-system, BlinkMacSystemFont, sans-serif;
  line-height: 1.6;
}
.page-header {
  display: none !important;
}
.hero {
  padding: 3.5rem 1.5rem 2rem;
  background: linear-gradient(145deg, #0d1b2a, #1b263b 60%, #415a77);
  border-radius: 1.25rem;
  color: #fff;
  text-align: center;
  box-shadow: 0 30px 60px rgba(15, 23, 42, 0.25);
}
.hero .eyebrow {
  text-transform: uppercase;
  letter-spacing: 0.3em;
  font-size: 0.8rem;
  color: rgba(255,255,255,0.7);
}
.hero h1 {
  margin: 0.5rem 0 1rem;
  font-size: clamp(2.4rem, 4vw, 3.7rem);
  color: var(--primary);
}
.hero p {
  margin: 0 auto 1.5rem;
  max-width: 680px;
  font-size: 1.05rem;
  color: rgba(255,255,255,0.85);
}
.hero-ctas {
  display: flex;
  justify-content: center;
  gap: 1rem;
  flex-wrap: wrap;
}
.btn {
  padding: 0.8rem 1.8rem;
  border-radius: 999px;
  font-weight: 600;
  border: 2px solid transparent;
  text-decoration: none;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}
.btn-primary {
  background: var(--primary);
  color: #fff;
  box-shadow: 0 10px 20px rgba(230, 57, 70, 0.35);
}
.btn-secondary {
  border-color: rgba(255,255,255,0.4);
  color: #fff;
}
.btn:hover {
  transform: translateY(-1px);
  box-shadow: 0 14px 26px rgba(17, 24, 39, 0.35);
}
.stat-row {
  margin: -1rem 0 2.5rem;
  display: grid;
  gap: 1rem;
  grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
}
.stat {
  background: var(--panel);
  padding: 1.2rem;
  border-radius: 0.9rem;
  box-shadow: 0 16px 30px rgba(0, 0, 0, 0.35);
  text-align: center;
  color: #e2e8f0;
}
.stat strong { font-size: 1.4rem; display: block; color: var(--secondary); }
.deck-title {
  margin: 3rem 0 1rem;
  font-size: 2rem;
  color: var(--secondary);
  text-align: center;
}
.tool-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
  gap: 1.5rem;
}
.card {
  background: var(--panel);
  border-radius: 1rem;
  border: 1px solid rgba(255,255,255,0.04);
  padding: 1.5rem;
  display: flex;
  flex-direction: column;
  gap: 0.8rem;
}
.card h3 { margin: 0; color: var(--secondary); }
.card p { color: var(--muted); margin: 0; }
.card a {
  margin-top: auto;
  font-weight: 600;
  color: var(--primary);
  text-decoration: none;
}
.detail {
  margin: 3rem 0;
  padding: 2rem;
  border: 1px solid var(--border);
  border-radius: 1.25rem;
  background: var(--panel);
  box-shadow: 0 22px 45px rgba(0,0,0,0.45);
  color: #e2e8f0;
}
.detail header h2 { margin: 0; color: var(--secondary); }
.detail header p { color: var(--muted); }
.detail-body {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1.5rem;
  margin-top: 1.5rem;
}
.tip, .extras {
  background: var(--panel-soft);
  border-radius: 0.9rem;
  padding: 1rem 1.2rem;
  border: 1px dashed var(--border);
}
.tip strong { color: var(--primary); }
.extras ul { padding-left: 1.2rem; margin: 0.5rem 0 0; }
.cta-banner {
  margin: 4rem 0 1rem;
  padding: 2rem;
  text-align: center;
  border-radius: 1rem;
  background: linear-gradient(120deg, #2b3e64, #1f2d46);
  color: #e2e8f0;
  box-shadow: 0 25px 35px rgba(0, 0, 0, 0.45);
}
</style>

<section class="hero">
  <h1>3DS Homebrew Hub</h1>
  <p>Four essential utilities with brief walkthroughs, presented as a living reference for anyone building a modded Nintendo 3DS setup.</p>
</section>

<section id="hshop" class="detail">
  <header>
    <h2>hShop - Titles & Themes</h2>
    <p>The go-to storefront replacement with simple filtering and in-app installs.</p>
  </header>
  <div class="detail-body">
    <div>
      <h4>Download flow</h4>
      <ol>
        <li>Launch hShop from the HOME Menu.</li>
        <li>Choose <strong>Games</strong> or <strong>Themes</strong> for your catalog.</li>
        <li>Select the <code>Europe (EUR)</code> region to list compatible entries.</li>
        <li>Browse the feed; anything shown is install-ready for that region.</li>
        <li>Highlight a title, tap <kbd>A</kbd>, then confirm with <kbd>A</kbd> again to install.</li>
      </ol>
    </div>
    <aside class="tip">
      <strong>Storage tip:</strong> The lower edge of the top screen tracks SD space in real time. Keep at least 1 GB free before queueing larger downloads to avoid mid-transfer failures.
    </aside>
  </div>
</section>

<section id="anemone" class="detail">
  <header>
    <h2>Anemone3DS - Theme Manager</h2>
    <p>Install, preview, or randomize custom themes in seconds.</p>
  </header>
  <div class="detail-body">
    <div>
      <h4>Install a theme</h4>
      <ol>
        <li>Launch Anemone3DS.</li>
        <li>Press <kbd>Y</kbd> to scan the SD card <code>/themes/</code> folder.</li>
        <li>Move with the D-pad to highlight a theme.</li>
        <li>Press <kbd>A</kbd> to install, then <kbd>Start</kbd> to exit and apply.</li>
      </ol>
    </div>
    <aside class="extras">
      <h4>Extras on deck</h4>
      <ul>
        <li>Randomize themes whenever the console wakes.</li>
        <li>Enable shuffle to rotate through your collection.</li>
        <li>Preview layouts before applying so you know what to expect.</li>
      </ul>
    </aside>
  </div>
</section>

<section id="luma" class="detail">
  <header>
    <h2>LumaLocaleSwitcher - Region Fixes</h2>
    <p>Force any installed title to the locale it needs, perfect for imported cartridges or eShop dumps.</p>
  </header>
  <div class="detail-body">
    <div>
      <h4>Apply a locale</h4>
      <ol>
        <li>Launch LumaLocaleSwitcher.</li>
        <li>Scroll through the installed titles list.</li>
        <li>Select the title that requires a locale override.</li>
        <li>Set <code>Region -> EUR</code> and <code>Language -> ENG</code> (or any combo you need).</li>
        <li>Confirm and exit, then launch the game - Luma applies the patch at boot.</li>
      </ol>
    </div>
    <aside class="tip">
      <strong>When to use:</strong> Imports that default to Japanese, region-locked DLC, or titles that refuse to boot outside a specific locale.
    </aside>
  </div>
</section>

<section id="fbi" class="detail">
  <header>
    <h2>FBI - Manual Installs</h2>
    <p>Homebrew's Swiss Army knife for handling CIA packages and SD file management.</p>
  </header>
  <div class="detail-body">
    <div>
      <h4>Install from SD</h4>
      <ol>
        <li>Launch FBI from the HOME Menu.</li>
        <li>Navigate with the D-pad and open <strong>SD</strong>.</li>
        <li>Browse to the folder housing the <code>.cia</code> (e.g., <code>/games/</code>).</li>
        <li>Select the CIA and choose <em>Install and delete</em> (or just <em>Install</em>).</li>
        <li>Once complete, the content appears alongside your other titles.</li>
      </ol>
    </div>
    <aside class="extras">
      <h4>Bonus tasks</h4>
      <ul>
        <li>Check tickets to confirm ownership.</li>
        <li>Delete outdated titles directly from the SD card.</li>
        <li>Use network install with an HTTP server for quicker transfers.</li>
      </ul>
    </aside>
  </div>
</section>
