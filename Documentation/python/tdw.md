# `tdw` module

`tdw` is a Python module that contains scripts that are mandatory for any controller.

## Installation

```bash
pip3 install tdw
```

## Contents

### Frontend

|                                                              | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Controller](https://github.com/threedworld-mit/tdw/blob/master/Documentation/python/controller.md) | Base class for all controllers.                              |
| [TDWUtils](https://github.com/threedworld-mit/tdw/blob/master/Documentation/python/tdw_utils.md) | Utility class.                                               |
| [AssetBundleCreator](https://github.com/threedworld-mit/tdw/blob/master/Documentation/python/asset_bundle_creator.md) | Covert 3D models into TDW-compatible asset bundles.          |
| [PyImpact](https://github.com/threedworld-mit/tdw/blob/master/Documentation/python/py_impact.md) | Generate impact sounds at runtime.                           |
| [DebugController](https://github.com/threedworld-mit/tdw/blob/master/Documentation/python/debug_controller.md) | Child class of `Controller` that has useful debug features.  |
| [KeyboardController](keyboard_controller.md)                 | Child class of `Controller` that can listen for keyboard input. |
| [Librarian](https://github.com/threedworld-mit/tdw/blob/master/Documentation/python/librarian/librarian.md) | "Librarians" hold asset bundle metadata records.             |
| [FluidTypes](https://github.com/threedworld-mit/tdw/blob/master/Documentation/python/fluid_types.md) | Access different NVIDIA Flex fluid types.                    |

### Backend

|                                                              | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| `flatbuffers/`                                               | Flatbuffer Python module.                                    |
| `FBOutput/`                                                  | TDW output data class types auto-generated by `TDWBase/Flatbuffer/compile.py`. These scripts are difficult to use! See `output_data.py`, which contains wrappers for each auto-generated class type. |
| `exe/`                                                       | Windows binaries used to create asset bundles.               |
| `backend/`                                                   | Misc. backend files.                                         |
| `metadata_libraries/`                                        | .json asset bundle records databases.                        |
| `asset_bundle_creator.unitypackage`                          | This file is used to generate a blank `asset_bundle_creator` Unity project. |
| `model_pipeline/`                                            | Specialized controllers used when creating model asset bundles. |
| [Build](https://github.com/threedworld-mit/tdw/blob/master/Documentation/python/build.md) | Helper functions for downloading the build.                  |
| [PyPi](https://github.com/threedworld-mit/tdw/blob/master/Documentation/python/pypi.md) | Helper functions for checking the version of the `tdw` module on PyPi. |