# RDL Proof-of-Concept Webapp

A simple example showcasing a GUI for a single set of hazard data.

For discussion purposes only.

# Dev setup

```bash
conda create -n rdl-webapp -c conda-forge python==3.8 mamba -y
conda activate rdl-webapp
mamba install -c conda-forge numpy==1.19.2 pandas==1.2.0 nodejs geopandas rasterio jupyterlab sidecar ipyleaflet voila -y
pip install ipyaggrid
python -m ipykernel install --name rdl-webapp --display-name "Python (rdl-webapp)"

jupyter labextension install @jupyter-widgets/jupyterlab-manager ipyaggrid

# These seem unneeded (?)
# jupyter labextension install js jupyter-leaflet @jupyter-widgets/jupyterlab-sidecar
```

## Required

A `.settings.yaml` file in the same format as [RISKi](https://github.com/ConnectedSystems/riski)