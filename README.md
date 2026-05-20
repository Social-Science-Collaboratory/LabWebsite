# Social Science Collaboratory — Lab Website

The official website of the **Social Science Collaboratory** at the University of Florida, directed by **Nicholas A. Coles**. The lab is dedicated to building and understanding big team science initiatives, with a focus on collective intelligence — both human and artificial.

Live site: [https://social-science-collaboratory.github.io/LabWebsite/](https://social-science-collaboratory.github.io/LabWebsite/)

---

## Research

### Studying Big Team Science

We track millions of scientific teams throughout the history of science to systematically understand the prevalence, impact, and drawbacks of large-scale research collaborations. Current work examines how scientists have responded to urgent societal developments including national security threats, global pandemics, and the rise of AI.

### Building Big Team Science

We run large multi-lab collaborations that tackle meaningful scientific questions, including:

- **The Many Smiles Collaboration** — 49 researchers across 19 countries studying the facial feedback hypothesis
- **The Global Gratitude Collaboration** — 36 researchers across 34 countries evaluating gratitude interventions
- **The Emotion Physiology and Experience Collaboration** — 51 researchers across 11 countries benchmarking machine learning for emotion prediction from physiology

### Supporting Big Team Science

We publish guides and advise large-scale initiatives, including the Psychological Science Accelerator, the Virtual Experience Research Accelerator, and the Global Happiness MegaStudy.

---

## Contact

For press inquiries, prospective PhD students, lab positions, or other questions, visit the [contact page](https://social-science-collaboratory.github.io/LabWebsite/contact/).

---

## Technical

**Stack:** Jekyll, [al-folio](https://github.com/alshedivat/al-folio) theme, hosted on GitHub Pages via branch deployment (`gh-pages` branch).

### Run locally with Docker

```bash
# Start the development server
docker compose pull && docker compose up
# Site runs at http://localhost:8080

# Rebuild after changing dependencies
docker compose up --build

# Stop the server
docker compose down
```
