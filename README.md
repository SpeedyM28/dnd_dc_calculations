# D&D Beyond Probability Calculator

A mobile‑friendly, client‑side web app for calculating dice‑pool success probabilities in Dungeons & Dragons (5e + homebrew).  
Perfect for quick, at‑the‑table maths—no backend, no sign‑up, just open the URL.

**Live demo:** `dnd-dc-calculations.vercel.app`

---

## Features

- **Dynamic dice pool** – add up to 10 dice, each chosen from d20, d12, d10, d8, d6, d4.
- **Modifier & target number** – standard attack/check parameters.
- **Natural 1 / Natural 20 rules** – optional toggles that match common house rules:
  - *Natural 1 always fails* (applies to the first die only, intended for d20s)
  - *Natural 20 always succeeds* (any die in the pool)
- **Multi‑attack calculator** – enter number of attacks, and specify how many have advantage / disadvantage.
- **Shareable URLs** – one click copies a link that fully restores your setup.
- **Dark mode** – toggle in the top‑right corner; preference saved locally.
- **Completely offline‑capable** – all calculations run in your browser; no data is sent anywhere.

> **⚠️ Note on advantage/disadvantage**  
> The calculator treats the **entire dice pool’s success probability** as one “roll”.  
> Advantage means “roll twice, take the higher probability”, rather than re‑rolling only the largest die.  
> This is an approximation for mixed dice (e.g., d20 + d8) and becomes exact when all dice are the same.

---

## How to use

1. **Set up your dice pool** – pick the number of dice and their types.
2. **Enter modifier and target** – e.g., `+5` to hit AC 15.
3. (Optional) Toggle **nat1 / nat20** rules if your table uses them.
4. Click **Calculate success probability** – you’ll see the chance for a single roll.
5. **Multi‑attack** section:
   - Enter how many attacks you make.
   - Set how many have advantage / disadvantage.
   - Click to get the probability that *all attacks succeed*.
6. **Copy link** – share your exact setup with your group or bookmark it.

---

## Tech stack

- Vanilla **HTML**, **CSS**, and **JavaScript**.
- No frameworks, no build step, no dependencies.
- Simple static files – deploy anywhere.

---

## Deployment

### Vercel (recommended)
1. Push the repository to GitHub.
2. Go to [vercel.com](https://vercel.com), sign in with GitHub.
3. Click **New Project** → import your repo.
4. Vercel will auto‑detect a static site; just click **Deploy**.
5. You’ll get a short URL like `dnd-calc.vercel.app`.

You can also deploy on **Netlify**, **GitHub Pages**, **Cloudflare Pages**, or any static host.

---

## Running locally

Just open `index.html` in your browser – no server required.

---

## File structure
├── index.html # Main HTML & JavaScript logic
├── style.css # All styles, including dark mode variables
└── README.md # This file

---

## Roadmap / possible additions

- [ ] Preset dice combinations (1d20, 2d20, d20+1d8, etc.)
- [ ] Restrict natural 1/20 rules to only d20 dice
- [ ] Visual dice roll distribution chart
- [ ] Save named profiles in localStorage

---

## License

MIT – feel free to use, modify, and share.
