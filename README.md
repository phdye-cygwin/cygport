# phdye-cygwin / cygport

Source-based Cygwin packages for the phdye-cygwin ports. Each directory
contains a cygport recipe that fetches the upstream vendor tarball, applies
Cygwin-specific patches, and builds installable Cygwin packages.

## Usage

```bash
cd abseil-cpp
cygport abseil-cpp-20250512.1-1.cygport download all
```

This fetches the upstream source, applies patches, compiles, runs tests,
and produces installable `.tar.xz` packages in the `dist/` directory.

## Packages

| Package | Upstream | Version | Patches |
|---------|----------|---------|---------|
| [abseil-cpp](abseil-cpp/) | [abseil/abseil-cpp](https://github.com/abseil/abseil-cpp) | 20250512.1 | 11 files |

## Layout

```
<package>/
  <package>-<version>-<release>.cygport    build recipe
  <package>-<version>-<release>.src.patch  Cygwin patches
  README                                   package description
```

## License

Each package retains its upstream license. The cygport recipes and patches
are provided under the same license as their respective upstream projects.
