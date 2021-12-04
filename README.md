# PhotogrametryTool

Generate 3D objects from images using RealityKit Object Capture. This project is a fork of the [HelloPhotogrametry](https://developer.apple.com/wwdc21/10076/) application by Apple, it ads various features such as USDZ to OBJ conversion and a progress bar.

## ⚠️ Requirements
 - macOS 12+ Monterey
 - An Apple Silicon Mac OR 
 - An Intel Mac with 16GB of RAM and an AMD GPU with 4GB of VRAM

## Usage
`$ photogrametrytool <input-folder> <output-filename> [--detail <detail>] [--sample-ordering <sample-ordering>] [--feature-sensitivity <feature-sensitivity>]`

### USDZ to OBJ Conversion
`$ photogrametrytool <input.usdz> <output-filename>`

## Options
| Shorthand | Flag                  | Available Options                   | Description                                                                                                                                                                 |
|-----------|-----------------------|-------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| -d        | --detail              | preview, reduced, medium, full, raw | Detail of output model in terms of mesh size and texture size.                                                                                                              |
| -o        | --sample-ordering     | unordered, sequential               | Setting to sequential may speed up computation if images are captured in a spatially sequential pattern. Set to unordered when you don't have good results with sequential. |
| -f        | --feature-sensitivity | normal, high                        | Set to high if the scanned object does not contain a lot of discernible structures, edges or textures.                                                                      |
| -h        | --help                |                                     | Show help information.                                                                                                                                                      |

## ToDo

- [ ] publish on homebrew
- [ ] -a flag that saves every quality setting
