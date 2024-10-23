# GLTF Model Library

A comprehensive library of optimized GLTF models for 3D rendering, including detailed assets with PBR materials, animations, and support for various levels of detail (LOD).

## Features

- **Optimized GLTF Models**: All models are optimized for performance in real-time rendering engines.
- **PBR Materials**: Models come with Physically Based Rendering (PBR) materials for realistic lighting and surface properties.
- **Animations**: Some models include animations, making them ready for use in dynamic scenes.
- **Level of Detail (LOD)**: Models support multiple levels of detail to improve rendering performance based on camera distance.

## Structure

The repository is organized in a structured way to make it easy to find and use models.

Example directory structure:

```
/gltf-models
  ├── model1
  │   ├── model1.gltf
  │   ├── model1.bin
  │   ├── textures/
  │       ├── albedo.png
  │       ├── normal.png
  │       └── roughness.png
  ├── model2
  │   └── ...
  └── modelN
```

Each model has its own folder with the following components:
- **GLTF (.gltf/.glb)**: The main model file.
- **Bin (.bin)**: Binary data file, if applicable.
- **Textures**: Folder containing related PBR textures such as albedo, normal, roughness, metallic, etc.

## Usage

These models can be used in any rendering engine that supports the GLTF format, including:

- **Three.js**
- **Babylon.js**
- **Blender**
- **Unity**
- **Unreal Engine**

To load and display a GLTF model in Three.js:

```javascript
const loader = new THREE.GLTFLoader();
loader.load('path/to/model.gltf', function(gltf) {
  scene.add(gltf.scene);
}, undefined, function(error) {
  console.error('An error occurred loading the model:', error);
});
```

## Contributions

We welcome contributions! If you want to add a model to the library or improve an existing model, please follow the contribution guidelines in `CONTRIBUTING.md`.

## License

All models in this repository are licensed under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/), unless otherwise stated.
