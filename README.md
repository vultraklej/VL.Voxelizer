# VL.Voxelizer

![Basic Demo](assets/media/basic-demo.png)

A **vvvv gamma** implementation of the mesh voxelization GPU algorithm originally from [mattatz/unity-voxel](https://github.com/mattatz/unity-voxel/tree/master), built using the **VL.Fuse**.

---

## Features

- Compatible with `ComputeSystem` and `GridSpace (3D)` sampling
- Supports arbitrary `AABB` (aka `AlignedBox`)
- Supports `TexCoords` and `Volume` sampling (as in the original implementation)

## Tested On
- VVVV Gamma: `7.0-0357`
- VL.Fuse: `1.0.3-beta06`

## Current Status

This project is currently under sporadic development and is not yet available as a packaged release. But that shouldn't stop you from experimenting with this algorithm🧪.

### Known Issues

- `TexCoords` sampling may produce jittered results between frames depending on the source model data

### Backlog

- [ ] Add support for vertex color sampling
- [ ] Merge shader into one using conditional compilation/effect permutation🤔
- [ ] Add more examples
- [ ] Replace SDSL implementation with pure `ComputeSystem`🗻