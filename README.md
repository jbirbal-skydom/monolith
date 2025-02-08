# Monolith

<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<!-- markdownlint-disable-file MD033 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/jbirbal-skydom/monolith">
    <img src="images/logo.gif" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">Monolith</h3>

  <p align="center">
    Next-generation color barcode system with 50x data density
    <br />
    <a href="https://github.com/jbirbal-skydom/monolith"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/jbirbal-skydom/monolith">View Demo</a>
    ·
    <a href="https://github.com/jbirbal-skydom/monolith/issues">Report Bug</a>
    ·
    <a href="https://github.com/jbirbal-skydom/monolith/issues">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://monolith.skydom.ai)

Monolith is revolutionizing how we store and transfer data in the physical world. By leveraging layered hexagonal color patterns, we've created a barcode system that can store up to 50x more data than traditional QR codes while being significantly more resilient to damage.

Key Features:

* 📦 **High Data Density**: Store up to 50x more data than traditional barcodes
* 🛡️ **Damage Resistant**: Maintains readability even with 30% physical damage
* 🎨 **Color Innovation**: Uses RGB/CMYK layers for enhanced data capacity
* 🔄 **Format Flexibility**: Supports text, URLs, binary data, and more
* 📱 **Universal Scanning**: Works with any RGB/CMYK-capable scanner

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

* [![Slint][slint-lang]][Slint-url]
* [![Rust][rust-lang]][Rust-url]
* [![C][c-lang]][C-url]
* [![GCC][gcc-badge]][GCC-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

* Rust
  
  ```sh
  curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
  ```

### Installation

1. Clone the repo
  
    ```sh
    git clone https://github.com/jbirbal-skydom/monolith.git
    cd monolith
    git submodule init
    git submodule update
   ```

2. Build the project
  
   ```sh
   cargo build --release
   ```

3. Run tests
  
   ```sh
   cargo test
   ```

### Monolith System Repositories

#### monolith

The main meta-repository that brings together all Monolith components. This repository uses Git submodules to manage the individual components and provides a unified build system for the entire Monolith ecosystem.

* **Purpose**: Project coordination, system-wide documentation, and integrated builds
* **Dependencies**: All other repositories as submodules
* **Key Features**: Workspace management, CI/CD pipelines, system-wide testing

#### [monolith-common](https://github.com/jbirbal-skydom/monolith-common)

Shared library containing common utilities, types, and interfaces used across all Monolith components.

* **Purpose**: Code reuse, standardization, and interface definitions
* **Key Features**: Crypto primitives, common traits, shared types, communication protocols
* **Used By**: All other Monolith components

#### [monolith-gui](https://github.com/jbirbal-skydom/monolith-gui)

The graphical user interface component for the Monolith system.

* **Purpose**: User interaction and data visualization
* **Dependencies**: monolith-common
* **Key Features**: Color pattern visualization, code generation interface, scanning interface

#### [monolith-core](https://github.com/jbirbal-skydom/monolith-core)

Core processing and coordination component of the Monolith system.

* **Purpose**: Central coordination and main business logic
* **Dependencies**: monolith-common
* **Key Features**: Request handling, component coordination, main processing pipeline

#### [monolith-data-process](https://github.com/jbirbal-skydom/monolith-data-process)

Data processing and analysis component.

* **Purpose**: Handle data transformation and processing
* **Dependencies**: monolith-common
* **Key Features**: Data validation, transformation, pattern recognition

#### [monolith-generator](https://github.com/jbirbal-skydom/monolith-generator)

Code generation and pattern creation component.

* **Purpose**: Generate Monolith codes and patterns
* **Dependencies**: monolith-common
* **Key Features**: Pattern generation, code optimization, error correction

#### [monolith-output](https://github.com/jbirbal-skydom/monolith-output)

Output handling and export component.

* **Purpose**: Handle final code output and export
* **Dependencies**: monolith-common
* **Key Features**: Output formatting, file export, printing preparation

#### [monolith-key-mgmt](https://github.com/jbirbal-skydom/monolith-key-mgmt)

Security and key management component.

* **Purpose**: Handle all cryptographic operations and key management
* **Dependencies**: monolith-common
* **Key Features**: Ephemeral key generation, key distribution, signature verification

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage

### Basic Example

```rust
use monolith::encoder;

let data = "Hello, Monolith!";
let code = encoder::generate(data, Options::default());
code.save("my_code.png")?;
```

### Scanning

```rust
use monolith::decoder;

let code = decoder::scan_from_image("code.png")?;
println!("Decoded data: {}", code.data());
```

_For more examples and usage, please refer to the [Documentation](https://docs.monolith.dev)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ROADMAP -->
## Roadmap

* [x] Core encoding/decoding engine
* [x] Basic RGB/CMYK support
* [x] Error correction implementation
* [ ] Mobile SDK
  * [ ] iOS Framework
  * [ ] Android Library
* [ ] Web Components
* [ ] Enterprise Features

See the [open issues](https://github.com/jbirbal-skydom/monolith/issues) for a full list of proposed features and known issues.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Project Link: [https://github.com/jbirbal-skydom/monolith](https://github.com/jbirbal-skydom/monolith)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [OpenCV Community](https://opencv.org/)
* [Rust Community](https://www.rust-lang.org/)
* [All Contributors](https://github.com/yourusername/monolith/contributors)
* [Sponsors](https://docs.monolith.skydom.ai/docs/resources/sponsorship)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/jbirbal-skydom/monolith.svg?style=for-the-badge
[contributors-url]: https://github.com/jbirbal-skydom/monolith/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/jbirbal-skydom/monolith.svg?style=for-the-badge
[forks-url]: https://github.com/jbirbal-skydom/monolith/network/members
[stars-shield]: https://img.shields.io/github/stars/jbirbal-skydom/monolith.svg?style=for-the-badge
[stars-url]: https://github.com/jbirbal-skydom/monolith/stargazers
[issues-shield]: https://img.shields.io/github/issues/jbirbal-skydom/monolith.svg?style=for-the-badge
[issues-url]: https://github.com/jbirbal-skydom/monolith/issues
[license-shield]: https://img.shields.io/github/license/jbirbal-skydom/monolith.svg?style=for-the-badge
[license-url]: https://github.com/jbirbal-skydom/monolith/blob/master/LICENSE.txt
[product-screenshot]: images/screenshot.png

 <!-- Badge  -->

[rust-lang]: https://img.shields.io/badge/Rust-f74c00?style=for-the-badge&logo=rust&logoColor=white
[Rust-url]: https://www.rust-lang.org/
[c-lang]: https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white
[C-url]: "https://en.wikipedia.org/wiki/C_(programming_language)"
[slint-lang]: https://img.shields.io/badge/Slint-7F52FF?style=for-the-badge&logo=slint&logoColor=white
[Slint-url]: https://slint-ui.com/
[gcc-badge]: https://img.shields.io/badge/GCC-4E9A06?style=for-the-badge&logo=gnu&logoColor=white
[GCC-url]: https://gcc.gnu.org/
