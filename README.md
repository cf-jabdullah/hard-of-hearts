# Anatomy 3D Assets

A collection of 3D anatomical models for interactive educational applications, medical visualizations, and browser-based 3D experiences.

This repository serves as a centralized asset library for AI agents and applications that use Three.js to render anatomical structures.

## Purpose

Provide accessible, reusable 3D assets that can be integrated into HTML, CSS, and JavaScript applications without requiring local 3D modeling software.

The repository supports:

- Interactive anatomical exploration
- Medical education and research visualizations
- AI-generated educational applications
- Browser-based 3D rendering
- Anatomical simulations and demonstrations

## Technology

- **Three.js:** Browser-based 3D rendering
- **GLTFLoader:** Loading GLB and GLTF models
- **JavaScript:** Model interaction and animation
- **GitHub:** Public hosting and distribution of 3D assets

## Repository Structure

```text
anatomy-3d-assets/
├── models/
│   ├── heart.glb
│   ├── brain.glb
│   ├── lungs.glb
│   └── kidney.glb
├── ATTRIBUTION.md
└── README.md
```

*The structure above is illustrative. Available models depend on the assets added to the repository.*

## Using the Models

Applications can retrieve publicly hosted GLB files using GitHub's raw file URLs.

Example URL:

```text
https://raw.githubusercontent.com/USERNAME/anatomy-3d-assets/main/models/MODEL.glb
```

Load the asset with Three.js:

```javascript
import { GLTFLoader } from 'three/addons/loaders/GLTFLoader.js';

const loader = new GLTFLoader();

loader.load(
  MODEL_URL,
  (gltf) => {
    scene.add(gltf.scene);
  },
  undefined,
  (error) => console.error('Model loading failed:', error)
);
```

Replace `MODEL_URL` with the actual hosted GLB URL.

## Asset Guidelines

Models added to this repository should:

- Use GLB format when possible.
- Preserve original geometry, materials, and textures.
- Include source attribution and licensing information.
- Be suitable for educational visualization.
- Have redistribution permissions verified before publication.

## Licensing and Attribution

Individual 3D models may have different licenses.

Refer to `ATTRIBUTION.md` for original creators, source URLs, license terms, and redistribution requirements.

Unless explicitly stated otherwise, this repository does not claim ownership of third-party anatomical assets.

## Educational Disclaimer

Models and visualizations in this repository are intended for educational and research demonstrations. Anatomical representations may contain simplifications and should not be used for medical diagnosis, clinical planning, or treatment decisions.
