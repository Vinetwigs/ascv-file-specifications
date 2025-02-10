
# ASCIIVideo (.ASCV) File Format Specification v1.1.0 

This repository contains the comprehensive specifications document of the **ASCIIVideo (`.ascv`) file** format, which enables encoding ASCII art sequences.
## Overview
The `.ascv` file format is designed to assist developers in implementing parsers and encoders/decoders for creating video files using ASCII characters.

### Key Features:
- **File Structure**: Consists of a header containing essential metadata (e.g., dimensions, frame rate) followed by the actual encoded frames.
  
  - `Header`: Fixed size at 32 bytes. Includes video properties like width and height.
    * Fields:
      | Field Name       | Type         | Size     |
      |------------------|--------------|----------------------------------------|
      | MAGIC            | String (4B)  | Identifies the file type, e.g., 'AAVF' |

- **Compression**: Supports DEFLATE compression to efficiently store video frames without compromising data integrity. The format allows for easy integration of encoding and decompression into existing software systems.

### Versioning
The version follows Semantic Versioning `1.X.Y`:
  - X (Major): Backward-incompatible changes like file structure alterations.
  - Y (Minor): Non-breaking additions such as new features or optimizations [source_id: ASVC_File_Format_Specifications.pdf].

## Getting Started

To utilize the `.ascv` format, refer to **ASCV File Format Specifications v1.1.0** available in this repository.
This document will guide you through implementing and utilizing ASCIIVideo files effectively, ensuring compliance with current standards of `.ascv` format encoding [source

## License
The specification PDF is provided under the BSD 3-Clause license.
