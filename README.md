# 3D Reconstruction → USD → Isaac Sim

End-to-end pipeline:
1) Open dataset ingestion (KITTI + Replica/NYU optional)
2) Train 3D Gaussian Splatting (Nerfstudio Splatfacto) and/or NeRF
3) Export reconstruction (PLY/OBJ/mesh)
4) Convert to USD
5) Load into Isaac Sim and record flythrough
6) Evaluate quality (PSNR + depth RMSE where ground truth exists)

## Repo Layout
- `scripts/` automation scripts for processing, training, export, conversion
- `notebooks/` analysis + plots (metrics, comparisons)
- `data/` local datasets (not committed)
- `outputs/` training outputs (not committed)
- `exports/` exported meshes/pointclouds (not committed)
- `usd/` final USD assets (keep small)
- `media/` demo videos and figures
- `docs/` calibration notes, coordinate frames, writeups

## Quickstart (coming next)
- Environment setup (conda)
- Nerfstudio install
- KITTI preprocessing
- Train Splatfacto
- Export + USD convert
- Isaac Sim load
