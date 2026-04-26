# Bin Packing · NP-Completeness · Greedy Algorithms

🔗 **[Live Demo](https://05nuha.github.io/Bin_Packing_Problem/)**

---

## About

This tool teaches Bin Packing — one of the most practical NP-complete problems — through interactive visualization, a full NP-completeness proof, and algorithm comparison. Built as a single HTML file with no external libraries.

---


## Features

- 🎨 **Waste heatmap** — empty bin space colored green→yellow→red by waste amount
- 🧠 **Quiz mode** — 12 questions across all 3 CLOs to test understanding
- ⚡ **Run All 4** — compare all algorithms on the same input instantly
- 📊 **Growth curve** — brute force vs FFD complexity chart
- 🔄 **Interactive reduction demo** — Partition → Bin Packing animated live
- 📖 **Learn tab** — full explanation from scratch, no textbook needed
- 4 presets covering different item distributions
- Custom input support
- Step/Play/Pause/Reset controls with speed slider

---

## Algorithms

| Algorithm | Time | Guarantee |
|-----------|------|-----------|
| Brute Force | O(kⁿ) | Exact optimal |
| First-Fit | O(n²) | ≤ (17/10)·OPT |
| Best-Fit | O(n²) | ≤ (17/10)·OPT |
| FFD | O(n log n) | ≤ (11/9)·OPT + 6/9 |

---

## Presets

| Preset | Items | Lesson |
|--------|-------|--------|
| Balanced | Mixed sizes | All algorithms tie — baseline |
| Small First | Ascending order | Sorting saves a bin |
| Awkward | 0.45×4, 0.55×4 | FFD=4, FF=6 — dramatic difference |
| Partition NP | 0.6, 0.6, 0.4, 0.4 | Reduction demo input |

---

## Tech Stack

- HTML5, CSS3, Vanilla JavaScript (ES6+)
- No external libraries or frameworks
- Single `.html` file — deploy anywhere

---

## Deploy on GitHub Pages

1. Upload `index.html` to a public GitHub repository
2. Go to **Settings → Pages → Source → main → / (root) → Save**
3. Your tool will be live at `https://<username>.github.io/<repo-name>/`

