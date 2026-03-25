# Lattice Hub

Structured toolkits for engineers — all in single, offline-ready HTML files.

## Lattices

| Lattice | Focus | File |
|---------|-------|------|
| **DesignLattice** | System design — diagrams, patterns, trade-offs, builders | `designlattice.html` |
| **CodeLattice** | Coding interviews — patterns, algorithm guides, interview sim | `codelattice.html` |

## Getting Started

Just open `index.html` in a browser. That's it — no build step, no dependencies.

### Deploy with GitHub Pages

1. Push this repo to GitHub
2. Go to **Settings → Pages → Source → Deploy from branch** (`main`, root `/`)
3. Your site is live at `https://<username>.github.io/lattice-hub/`

## Adding a New Lattice

1. Create your `newlattice.html` in the root
2. Add a card to `index.html` inside `<section class="lattice-grid">`:

```html
<a href="./newlattice.html" class="lattice-card" data-accent="purple">
  <div class="card-top">
    <div class="card-icon">⬡</div>
    <span class="card-arrow">↗</span>
  </div>
  <div class="card-body">
    <span class="card-subtitle">Category</span>
    <div class="card-title">NewLattice</div>
    <div class="card-desc">What this lattice covers.</div>
  </div>
  <div class="card-tags">
    <span class="card-tag">tag1</span>
    <span class="card-tag">tag2</span>
  </div>
</a>
```

Available accent colors: `blue`, `green`, `purple`, `amber`.

3. Add a hub button in your new lattice's topbar:

```html
<a href="./index.html" class="home-btn" style="text-decoration:none;margin-right:4px">◇ Hub</a>
```

## License

Open source.
