# M-Lab CARTE AI Workshop 2025 — Participant Archive

This repository hosts the full set of materials from the University of Toronto CARTE four-day workshop. Use it as a self-paced refresher: stream lecture recordings, review slide decks, and re-run the lab exercises with guided practice prompts and solutions.

## Repository Layout

- `docs/` — Source for the GitHub Pages site (`docs/index.md` is the homepage).
- `labs/` — Interactive Jupyter notebooks (`.ipynb`) plus printable PDF handouts.
- `lab-d-output/` — Showcase outputs from the multimodal lab teams.
- `slides/` — All lecture and workshop slide decks, ready to download.
- `assets/` — Supporting media referenced by the labs and docs.

## Getting Started

### Option 1: Run in Google Colab (easiest)

1. Open the lab of interest using the “Open in Colab” link on the [workshop homepage](docs/index.md).
2. In Colab, choose `File → Save a copy in Drive` to keep your own editable version.
3. Run the notebook cells in sequence, completing the `TODO` prompts. Solution callouts are embedded near each task.

### Option 2: Run locally with Python

1. Clone the repository and create a fresh virtual environment.
2. Install the Python dependencies listed in `requirements.txt`.
3. Start Jupyter:
   ```bash
   jupyter lab
   ```
4. Open the lab notebook (`labs/lab_a_exploratory_data_analysis.ipynb`, etc.), work through the prompts, and compare with the included solutions.

## Environment Notes

- Python 3.10+ is recommended. Earlier versions may work but are not actively tested.
- Install packages with `pip install -r requirements.txt`. This captures the core libraries used across all labs: NumPy, pandas, Matplotlib, scikit-learn, ydata-profiling, and imbalanced-learn.
- The Lab B notebook also demonstrates the optional `ydata-sdk` install command for generating rich profiling reports. The requirements file already covers its dependencies; you do not need to run `!pip install ...` locally unless you want the latest release.
- JupyterLab or the classic notebook interface both work. Launch either via `jupyter lab` or `jupyter notebook` once your environment is activated.

## Workshop Materials at a Glance

- **Recordings & Quick Links:** The schedule in `docs/index.md` links directly to every lecture recording, slide deck, and lab.
- **Lecture Slides:** Browse or download printable PDFs from `slides/`.
- **Lab Notebooks:** `labs/` contains the live notebooks with TODO prompts, context, and inline solutions. The paired PDFs are ideal for executive summaries.
- **Multimodal Gallery:** Explore participant outputs from Lab D inside `lab-d-output/`.

## Need Help?

The final section of `docs/index.md` lists the CARTE team contacts. Reach out if you have follow-up questions, would like to share implementation learnings, or need updated credentials for future cohorts.

