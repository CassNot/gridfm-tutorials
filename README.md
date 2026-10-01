<p align="center">
  <img src="https://raw.githubusercontent.com/gridfm/gridfm-graphkit/refs/heads/main/docs/figs/KIT.png" alt="GridFM" width="280">
</p>

<h1 align="center">GridFM tutorials</h1>

<p align="center">
  Notebooks for looking at a grid foundation model: what it reconstructs, and how it behaves when lines are taken out.
</p>

<p align="center">
  <a href="https://colab.research.google.com/github/gridfm/gridfm-tutorials/blob/main/notebooks/Tutorial_reconstruction_visualization.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open the reconstruction tutorial in Colab"></a>
  &nbsp;
  <a href="https://colab.research.google.com/github/gridfm/gridfm-tutorials/blob/main/notebooks/Tutorial_contingency_analisys.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open the contingency tutorial in Colab"></a>
</p>

The library itself stays in [gridfm/gridfm-graphkit](https://github.com/gridfm/gridfm-graphkit). These notebooks are the walkthrough.

## State reconstruction

[Open in Colab](https://colab.research.google.com/github/gridfm/gridfm-tutorials/blob/main/notebooks/Tutorial_reconstruction_visualization.ipynb) · [notebook](notebooks/Tutorial_reconstruction_visualization.ipynb)

IEEE 30. One load scenario. The notebook draws the grid and paints each bus by the active-power residual, then by the reconstructed demand, generation, voltage magnitude, and voltage angle.

It reads `config/case30_ieee_base.yaml`, a case30 dataset, and `models/GridFM_v0_2.pth` from the directory above the notebook. Colab installs `gridfm-graphkit` for you.

## Contingency analysis

[Open in Colab](https://colab.research.google.com/github/gridfm/gridfm-tutorials/blob/main/notebooks/Tutorial_contingency_analisys.ipynb) · [notebook](notebooks/Tutorial_contingency_analisys.ipynb)

Ten N-2 scenarios on the Texas grid, saved in [`data/contingency_texas/`](data/contingency_texas/). The notebook compares GridFM line loading and voltage with AC power flow and with DC power flow: correlation plots, confusion matrices, and where the error sits along the loading range.

Colab installs `gridfm-graphkit` and clones this repo so it can see those files.

## Run it here

```bash
pip install gridfm-graphkit
```

Then open either notebook. From this repo, the contingency sample is at `data/contingency_texas/`.
