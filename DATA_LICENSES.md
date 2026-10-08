# Data licenses

Benchmark taskpacks reference third-party datasets under their original terms (USGS, NOAA, Zenodo-hosted challenge data, etc.). Redistributable excerpts included in this repository are marked in taskpack metadata where applicable.

Model weights (Llama, Gemma, Mixtral, OLMo, DeepSeek API) require separate acceptance of each provider's license before download.

## Third-party software

### SFINCS

[SFINCS](https://www.deltares.nl/en/software-and-data/products/sfincs) (Super-Fast INundation of CoastS) is a reduced-physics hydrodynamic model for compound flooding developed by [Deltares](https://www.deltares.nl/en). It is used by the `CAP-FL2-04` and `CAP-MH3-01` capabilities. SFINCS is not redistributed here: the source is fetched from <https://github.com/Deltares/SFINCS> and the model is run through the official `deltares/sfincs-cpu` container, both under their original terms (GNU GPL v3.0 for the source). The MIT license of this repository does not apply to SFINCS.

- Website: <https://www.deltares.nl/en/software-and-data/products/sfincs>
- User manual: <https://sfincs.readthedocs.io>
- Source: <https://github.com/Deltares/SFINCS>

If you use the SFINCS-backed routes, please cite:

```bibtex
@article{leijnse2021sfincs,
  title   = {Modeling compound flooding in coastal systems using a computationally efficient reduced-physics solver: Including fluvial, pluvial, tidal, wind- and wave-driven processes},
  author  = {Leijnse, Tim and van Ormondt, Maarten and Nederhoff, Kees and van Dongeren, Ap},
  journal = {Coastal Engineering},
  volume  = {163},
  pages   = {103796},
  year    = {2021},
  doi     = {10.1016/j.coastaleng.2020.103796}
}
```
