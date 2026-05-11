# OGR-TE-Validation

**Orthogonal Validation of Transposable Element Polymorphisms Using a Rice Genomic Foundation Model**

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX)

This repository contains the analysis code and data for the manuscript:

> *Genomic Foundation Models Reveal Chromatin-Domain-Scale Transposable Element Impacts on Rice Genome Architecture*

Submitted to *The Plant Cell*.

## Contents

### Scripts
- `scripts/build_p5_plantcell_v2.py` — Build the complete manuscript Word document with embedded figures
- `scripts/p5_figures_plantcell.py` — Generate publication-quality TIFF figures (300 PPI, Arial, RGB)
- `scripts/p5_kmer_baseline.py` — Non-neural baseline comparison (k-mer spectra, GC content)

### Data
- `data/ogr_sliding_window.json` — OGR embedding sliding-window analysis results (22 windows, Chr04:1.1–5.5 Mb)
- `data/p5_baseline_results.json` — Multi-baseline comparison results (OGR vs 6-mer vs GC content)

### Output
- `output/P5_Fig1_CTB4a_Validation.tiff` — CTB4a locus validation (Figure 1)
- `output/P5_Fig2_SlidingWindow.tiff` — Three-track sliding window analysis (Figure 2)
- `output/P5_Fig3_Framework.tiff` — GFM validation framework (Figure 3)

## Dependencies

- Python 3.10+
- PyTorch 2.8+
- NumPy 1.26+
- SciPy 1.16+
- matplotlib 3.9+
- python-docx 1.1+
- OneGenome-Rice model weights (see `https://github.com/[ogr-repo]`)

## Usage

```bash
# Generate figures
python scripts/p5_figures_plantcell.py

# Run baseline comparison
python scripts/p5_kmer_baseline.py

# Build manuscript Word document
python scripts/build_p5_plantcell_v2.py
```

## License

MIT License. See `LICENSE` file.

## Citation

If you use this code or data, please cite:
> [Authors]. Genomic Foundation Models Reveal Chromatin-Domain-Scale Transposable Element Impacts on Rice Genome Architecture. *The Plant Cell* (2026).
