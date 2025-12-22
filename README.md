<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width,initial-scale=1">
    <title>quandnexusy — README</title>
    <style>
      body{font-family:Inter,Arial,Helvetica,sans-serif;background:#0f1724;color:#e6eef6;padding:24px}
      .card{max-width:900px;margin:24px auto;padding:24px;background:#0b1220;border:1px solid #1f2937;border-radius:12px}
      h1{color:#7dd3fc;margin-bottom:4px}
      p{color:#cbd5e1}
      code{background:#071026;padding:2px 6px;border-radius:6px;color:#99f6e4}
      pre{background:#071026;padding:12px;border-radius:8px;overflow:auto}
      a{color:#7dd3fc}
    </style>
  </head>
  <body>
    <main class="card">
      <h1>quandnexusy</h1>
      <p>A lightweight React + Firebase discussion feed originally named QuantumNexus. This repository contains the single-page UI component used by the project.</p>

      <h2>Quick Start</h2>
      <ol>
        <li>Install dependencies (typical for React projects):
          <pre><code>npm install
# or
pnpm install</code></pre>
        </li>
        <li>Provide Firebase config and optional tokens in the embedding environment:
          <pre><code>// Example globals required by the app (in the host HTML or server-side render)
window.__firebase_config = JSON.stringify({ /* your firebase config */ });
window.__app_id = 'your-app-id';
// optional
window.__initial_auth_token = 'CUSTOM_TOKEN';
</code></pre>
        </li>
        <li>Run the dev server:
          <pre><code>npm run dev
# or
pnpm dev</code></pre>
        </li>
      </ol>

      <h2>Important Files</h2>
      <ul>
        <li><a href="quantumnexus001">Main UI component</a> — single-file React component rendering the feed and UI.</li>
        <li><a href="README.md">This README</a></li>
      </ul>

      <h2>Notes</h2>
      <ul>
        <li>The visible site title has been updated to <strong>quandnexusy</strong> in the UI.</li>
        <li>Data is stored under Firestore paths that include the app id; update <code>window.__app_id</code> appropriately for multi-tenant deployments.</li>
        <li>Images are limited to ~500KB in the UI to avoid large Firestore documents.</li>
      </ul>

      <h2>Want me to…</h2>
      <ul>
        <li>Update README to plain Markdown instead of HTML? (I can convert it.)</li>
        <li>Search & replace remaining mentions of the old name in filenames/metadata?</li>
      </ul>
    </main>
  </body>
</html>
