# Bin Packing · NP-Completeness · Greedy Algorithms

**Nuha Aburamadan** | BCS 309 Algorithms I — Spring 2026  
Interactive step-by-step algorithm visualizer built for the final project.

🔗 **[Live Demo](https://05nuha.github.io/your-repo-name/)**

---

## About

This tool teaches Bin Packing — one of the most practical NP-complete problems — through interactive visualization, a full NP-completeness proof, and algorithm comparison. Built as a single HTML file with no external libraries.

---

## What It Covers

### CLO-5 — NP-Completeness Proof
- Step-by-step proof that Bin Packing is in NP (certificate + verifier)
- Polynomial-time reduction from Partition → Bin Packing
- Forward and backward directions proved with concrete examples
- Interactive reduction demo with live animation

### CLO-4 — Algorithm Visualization
- **Brute Force** — exact optimal via backtracking
- **First-Fit** — greedy, original order
- **First-Fit Decreasing (FFD)** — greedy, sorted largest-first
- **Best-Fit** — greedy, tightest packing
- Step-by-step animation with pseudocode highlighting
- Side-by-side comparison of all 4 algorithms

### CLO-3 — Algorithm Design
- Greedy paradigm identified and justified
- Why sorting in decreasing order helps (large items first)
- Approximation ratio (11/9)·OPT explained with proof sketch
- Counterexample showing FFD is not always optimal
- Waste heatmap showing packing efficiency visually

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

## How to Use

1. Choose an algorithm mode from the left panel
2. Load a preset or enter custom item sizes (space-separated, between 0 and 1)
3. Click **Build Steps** to generate the animation
4. Click **Step ▶** to go one step at a time, or **Play** to animate automatically
5. Hover any pseudocode line for a detailed explanation
6. Click **⚡ Run All 4** to compare all algorithms side by side
7. Switch to the **Learn tab** → **🧠 Test my understanding** to take the quiz

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

---

## References

- Garey, M. R. & Johnson, D. S. (1979). *Computers and Intractability*. W. H. Freeman.
- Johnson, D. S. (1973). Near-optimal bin packing algorithms. PhD thesis, MIT.
- Simchi-Levi, D. (1994). New worst-case results for the bin-packing problem. *Naval Research Logistics*, 41(4).
- Karp, R. M. (1972). Reducibility among combinatorial problems. *Complexity of Computer Computations*.
