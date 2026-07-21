# BRAINSTools

A CMake SuperBuild harness providing a suite of command-line tools for
brain MRI processing — registration, segmentation, atlas generation, DWI
processing, and defacing. Developed at the University of Iowa and also
distributed as part of [3D Slicer](https://www.slicer.org/).

**Documentation: <https://brainsia.github.io/BRAINSTools/>**

- [Tool catalog](https://brainsia.github.io/BRAINSTools/tools.html)
- [Wiki](https://github.com/BRAINSia/BRAINSTools/wiki)

## Quick start

```sh
git clone https://github.com/BRAINSia/BRAINSTools.git
cmake -S BRAINSTools -B BRAINSTools-build -DCMAKE_BUILD_TYPE=Release
cmake --build BRAINSTools-build
```

The SuperBuild fetches and builds dependencies (ITK, VTK, ANTs, …)
automatically, then builds the BRAINSTools. On macOS, first install the
command line tools with `xcode-select --install`.

## Contributing

Run `./Utilities/SetupForDevelopment.sh`, then `pre-commit install`.
See [CONTRIBUTING.md](.github/CONTRIBUTING.md).

## License

Apache 2.0. See [LICENSE](LICENSE).
