# CLAUDE.md - Awesome-Latent-Space

## Description

Curated paper list on latent space reasoning for LLMs, VLMs, VLAs, World Models, and Multi-Agent Systems. Fork of YU-deep/Awesome-Latent-Space.

## What This Is

- 107 papers organized in 5 categories (LLM: 58, VLM: 24, VLA: 13, WM: 7, MAS: 5)
- 105 PDFs downloaded (~542 MB) in PAPERS/
- 109 method diagrams in img/ (~15 MB)
- Analysis scripts: download_papers.sh, build_index.py, analyze_papers.py

## Structure

```
Awesome-Latent-Space/
├── README.md              # Main paper catalog (173 lines)
├── PAPERS/                # Downloaded PDFs + analysis tools
│   ├── *.pdf              # 105 papers by arXiv ID
│   ├── build_index.py     # Generates index.json/csv from README
│   ├── analyze_papers.py  # Trend analysis, bigrams, conferences
│   └── download_papers.sh # Batch PDF downloader from arXiv
├── img/                   # Method diagrams by category
│   ├── llm/ vlm/ vla/ wm/ mas/ static/
├── CONTRIBUTING.md
└── LICENSE                # MIT
```

## Analysis Tools

```bash
# Download missing PDFs
bash PAPERS/download_papers.sh

# Build index from README
python PAPERS/build_index.py

# Analyze trends
python PAPERS/analyze_papers.py
```

## Key Numbers

- 586 MB total repo size
- 66 commits, 8 contributors (Nov 2025 - Jan 2026)
- 12 papers accepted at top conferences (ICML, ICLR, NeurIPS, EMNLP, ACL)

## Known Issues

- Scripts have hardcoded absolute paths (not portable)
- PAPERS/analisis/ contains metadata from Agent-Memory-Paper-List (wrong repo, artifact)
- Duplicate URL in README for paper 2505.13308
- 2 papers appear in multiple categories (2509.18428, 2512.10226)
- No .gitignore (PDFs should use Git LFS)
- No requirements.txt (PyPDF2 is optional dependency)
