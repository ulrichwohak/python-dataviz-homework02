# Week 2 homework

The question and submission instructions are in [assignment.pdf](assignment.pdf).

## Setup

1. Open [the homework repository](https://github.com/ulrichwohak/python-dataviz-homework02).
2. Click **Fork**, select your own GitHub account as the owner, keep the repository
   name, and click **Create fork**.
3. Clone your fork to your computer, replacing `YOUR-USERNAME` with your GitHub username:

```bash
git clone https://github.com/YOUR-USERNAME/python-dataviz-homework02.git
cd python-dataviz-homework02
```

From this folder, set up the environment and launch JupyterLab:

```bash
uv sync --locked
uv run jupyter lab
```

Open `analysis.ipynb` and select the **Python 3 (ipykernel)** kernel.
Run the notebook from the repository root so its relative data path works.

The data are included in [data/working_time.csv](data/working_time.csv).
Variable definitions and provenance are in [data/README.md](data/README.md).

The course's **use AI, then verify** policy applies. Include a brief disclosure of
material AI assistance and how you checked it in the figure notes, or state that
there was none.

Original course material and code: MIT licence, as in [LICENSE](LICENSE).
The BLS source data are public domain. AI assistance was used to prepare the brief
and starter files; calculations were checked against the source data and published
BLS statistics.
