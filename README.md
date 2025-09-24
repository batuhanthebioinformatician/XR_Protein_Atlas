# XR Protein Atlas Viewer

An interactive web-based atlas for exploring **Xanthorhodopsin (XR) protein structures**.  
This tool allows researchers and students to visualize ~250 modeled XR proteins, grouped into **HDBSCAN clusters** derived from polymorphism and sequence similarity analysis.

## Features
- **3D interactive visualization** using [3Dmol.js](https://3dmol.org).
- **Navigation controls**: browse proteins with *Next* / *Prev* buttons.
- **Search bar**: look up proteins by **ID** or **cluster number**.
- **Cluster filters**: quickly focus on proteins grouped by clustering analysis.
- **Metadata panel**: displays protein ID and cluster information (more metadata coming soon).

## Data
- **Protein structures (.pdb)** were modeled computationally from XR sequences.  
- Sequences are classified into **clusters (-1 to 5)** according to machine learning–based analysis of BLOSUM45 similarity and polymorphisms.  
- Strains include Arctic, temperate, and plant-associated *Sphingomonas faeni* isolates, and additional XR sequences from NCBI.

## Deployment
This project is deployed on **GitHub Pages**:  
👉 [XR Protein Atlas](https://batuhanthebioinformatician.github.io/XR_Protein_Atlas/)

## Local Usage
To run locally:
```bash
# Clone the repo
git clone https://github.com/batuhanthebioinformatician/XR_Protein_Atlas.git
cd XR_Protein_Atlas

# Serve with Python (for local testing)
python -m http.server 8000
Then open: http://127.0.0.1:8000/index.html
