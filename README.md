---
title: NASA 3D Resources Viewer
emoji: "🚀"
colorFrom: indigo
colorTo: cyan
sdk: static
app_file: index.html
pinned: false
license: other
---

NASA-3D-Resources
=================

Welcome to the 3D Resources github site. This is a growing collection of 3D models, textures, and images from inside NASA. Our goal is to provide a comprehensive repository for 3D models, images, textures, and visualizations. These assets are free and without copyright.

Please read the [usage guidelines][usage]. NASA [intranet interface][webinterface] for these resources.

We welcome feedback and comments. Tell us how you're using our models and let us know what you think: arc-special-proj@lists.nasa.gov

## Quick start (local viewer)

Run a simple static server from the repository root and open the included viewer:

```bash
python3 -m http.server 8080
# then open http://localhost:8080/index.html
```

Use the dropdown or paste any relative GLB path (for example `3D Models/1999 RQ36 asteroid/1999 RQ36 asteroid.glb`) to inspect models with the built-in WebGL viewer.

## Deploy to Hugging Face Spaces (static)

1. Create a new Space set to **Static**. Example: `huggingface-cli repo create nasa-3d-resources-viewer --type=space --sdk=static`
   - If you have not authenticated locally: `huggingface-cli login --token <your-hf-token>`
2. Push this repository to that Space (replace `<your-hf-username>` as needed):
   ```bash
   git clone https://huggingface.co/spaces/<your-hf-username>/nasa-3d-resources-viewer
   cd nasa-3d-resources-viewer
   # add this repo as a remote and pull its contents
   git remote add origin-github https://github.com/souvikdhua/NASA-3D-Resources.git
   git pull origin-github main  # if your branch differs, replace "main" accordingly
   git push origin main
   ```
   (If the Space uses `main` instead of `master`, adjust accordingly.)
3. Once pushed, the Space automatically serves `index.html` with no extra build steps.

## Contributors

We thank the many authors who have contributed to the 3D Resources collections.

| Contributor                                             | Organization        |
| ------------------------------------------------------- | ------------------- |
| NASA Ames Research Center                               | NASA ARC            |
| NASA Goddard Space Flight Center                        | NASA GSFC           |
| NASA Jet Propulsion Laboratory                          | NASA JPL            |
| NASA Jet Propulsion Laboratory - Solar System Simulator | NASA JPL            |
| NASA Johnson Space Center                               | NASA JSC            |
| NASA Johnson Space Center - Space Educators' Handbook   | NASA JSC            |
| Ball Aerospace                                          |                     |
| DigitalSpace Corporation                                |                     |
| Eyes on the Solar System                                | NASA/JPL-Caltech    |
| Berry, Dana                                             | NASA/Kepler Mission |
| Carbajal, Michael                                       | NASA Headquarters   |
| Conti, Carlo                                            |                     |
| Ellison, Doug                                           | NASA JPL            |
| Garcia, Christopher M.                                  | NASA/JPL-Caltech    |
| Kumanchik, Brian                                        | NASA/JPL-Caltech    |
| Lane, Kevin                                             | NASA/JPL-Caltech    |
| Lopez, Christian A.                                     | NASA/JPL-Caltech    |
| Meaney, Chris                                           | NASA GSFC           |

[usage]: https://www.nasa.gov/nasa-brand-center/images-and-media
[webinterface]: https://nasa3d.arc.nasa.gov
