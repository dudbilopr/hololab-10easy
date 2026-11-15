# HoloLab10.easy — Interactive 3D Virtual Digital Holography Laboratory

Web-ready deployment bundle of **`HoloLab10.easy`**, an interactive Three.js / WebGL 3D digital twin for digital holography education and optical bench verification, paired numerically with [`holom-core`](https://github.com/dudbilopr/holom-core).

## Optical Setups Included
1. **Mach-Zehnder Fresnel Digital Holography** (off-axis recording & numerical reconstruction, zero-order suppression).
2. **2F Fourier CGH System with LCoS SLM** (Holoeye LC-R 2500 reflection setup, spatial filtering).
3. **Joint Transform Correlator (JTC) Optical Encryption** (joint power spectrum & phase-mask decryption).

## Features
- Real-time 3D optical bench geometry with physical catalog dimensions, specular reflections, and adjustable room illumination ("lights off" beam alignment mode).
- Integrated live **Physical Self-Check** (law of reflection, focal constraints, Nyquist carrier limit, beam path consistency).
- Real-time browser **Digital Twin** (Fresnel FFT reconstruction, zero-order filters, 4-step phase shifting, Gerchberg-Saxton).
- Embedded experimental reference holograms and reconstructions.

## Local Preview & Web Deployment
`index.html` is a self-contained static HTML5 application (zero build step required):

```bash
python -m http.server 8000
# Open http://localhost:8000/
```

Compatible directly with **GitHub Pages**, **Cloudflare Pages**, and **Netlify** (includes `.nojekyll`).

## Authorship & Licensing
- **Author & Design:** Dudbil Olvasada Pabón Riaño · **10.Easy** (`physics.10easy`)
- **ORCID:** [`0000-0001-7239-3497`](https://orcid.org/0000-0001-7239-3497)
- **License:** Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (**CC BY-NC-SA 4.0**) for the interactive simulator interface and educational assets, preserving commercial licensing flexibility under the `10.Easy` brand. For commercial or institutional licensing inquiries, contact `dudbilopr@gmail.com`.
- **Core Numerical Package:** Verified Python/PyTorch propagators, filters, and audits live in [`holom-core`](https://github.com/dudbilopr/holom-core) (`Apache-2.0`).
