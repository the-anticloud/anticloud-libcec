# LIBCEC

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-consumer_electronics-lightgrey)

> Anticloud-hardened packaging of the upstream project `LIBCEC` in category **CONSUMER ELECTRONICS**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** CONSUMER ELECTRONICS · **Upstream:** https://github.com/bramp/libcec-daemon · **Upstream pin:** `fe9df5ddf7356daa521f893c16872a09c8e6fb59` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

![Pulse-Eight logo](https://pulseeight.files.wordpress.com/2016/02/pulse-eight-logo-white-on-green.png?w=200)

# About
This library provides support for Pulse-Eight's USB-CEC adapter and other CEC capable hardware, like the Raspberry Pi.

A list of FAQ (Frequently Asked Questions) can be found on [libCEC's FAQ page](http://libcec.pulse-eight.com/faq).

.Net client applications, previously part of this project, have been moved to [this project](https://github.com/Pulse-Eight/cec-dotnet).

# API documentation

Full API reference — with install and usage guides — for every binding is
published at **[pulse-eight.github.io/libcec](https://pulse-eight.github.io/libcec/)**:

* [C / C++](https://pulse-eight.github.io/libcec/cpp/) — the native `ICECAdapter` interface and the C API
* [.NET](https://pulse-eight.github.io/libcec/dotnet/) — the managed `LibCecSharp` binding
* [Node.js](https://pulse-eight.github.io/libcec/nodejs/) — the N-API addon
* [Python](https://pulse-eight.github.io/libcec/python/) — the SWIG `cec` module
* [Rust](https://pulse-eight.github.io/libcec/rust/) — the `libcec` crate

The docs are generated from this source tree; see [docs/api/README.md](docs/api/README.md).

# Packages

Three bindings are published to their language's registry, from 8.1.6 onwards.
Each binds the native library rather than containing it, so libCEC itself still
has to be installed — see the platform sections below.

| | install | |
|---|---|---|
| .NET | `dotnet add package LibCecSharp` | [nuget.org](https://www.nuget.org/packages/LibCecSharp) |
| Node.js | `npm install libcec` | [npmjs.com](https://www.npmjs.com/package/libcec) |
| Rust | `cargo add libcec` | [crates.io](https://crates.io/crates/libcec) |

C, C++ and Python come from the platform packages: `libcec8-dev` and
`python-libcec` on Debian/Ubuntu, or the Windows installer.

# Supported platforms

## Linux & BSD
See [docs/README.linux.md](docs/README.linux.md).

## Apple OS X
See [docs/README.osx.md](docs/README.osx.md).

## Microsoft Windows
See [docs/README.windows.md](docs/README.windows.md).

# Supported hardware
* [Pulse-Eight USB-CEC Adapter](https://www.pulse-eight.com/p/104/usb-hdmi-cec-adapter)
* [Pulse-Eight Intel NUC CEC Adapter](https://www.pulse-eight.com/p/154/intel-nuc-hdmi-cec-adapter)
* [Pulse-Eight CEC Adapter for Skull Canyon and Hades Canyon NUC systems](https://www.pulse-eight.com/p/207/skull-canyon-nuc-cec-adapter)
* [Raspberry Pi](https://www.raspberrypi.org/)
* Some Exynos SoCs
* NXP TDA995x
* Odroid C2 (Amlogic S905)

# Developers
See [docs/README.developers.md](docs/README.developers.md).

# Vendor specific notes

## Panasonic
* On Panasonic to enable media control buttons on bottom of the remote, you may have to change the operation mode. To change it, press bottom Power-button, keep it pressed, and press 7 3 Stop. After releasing Power-button, Play, Pause, etc should work in XBMC.

## Raspberry Pi
* If your TV cannot detect the Raspberry Pi's CEC, or if the the Pi can't detect the TV, try adding the following line in `/boot/config.txt` and reboot the Pi: `hdmi_force_hotplug=1`

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **C/C++ / CMake** (manifests: CMakeLists.txt; scanned in UPSTREAM_CLONE)
- Top-level source layout: `cmake/`, `debian/`, `include/`, `licenses/`, `project/`, `src/`, `support/`, `systemd/`, `windows/`
- Snapshot size: **286 files**, **54410 lines of code** (measured; see Benchmarks)
- Primary languages: `.h` (79), `.cpp` (52), `(none)` (19), `.md` (18), `.py` (15), `.rs` (14)
- Upstream commit pinned for this packaging: `fe9df5ddf7356daa521f893c16872a09c8e6fb59`

---

## Installation

published at **[pulse-eight.github.io/libcec](https://pulse-eight.github.io/libcec/)**:

* [C / C++](https://pulse-eight.github.io/libcec/cpp/) — the native `ICECAdapter` interface and the C API
* [.NET](https://pulse-eight.github.io/libcec/dotnet/) — the managed `LibCecSharp` binding
* [Node.js](https://pulse-eight.github.io/libcec/nodejs/) — the N-API addon
* [Python](https://pulse-eight.github.io/libcec/python/) — the SWIG `cec` module
* [Rust](https://pulse-eight.github.io/libcec/rust/) — the `libcec` crate

The docs are generated from this source tree; see [docs/api/README.md](docs/api/README.md).

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

published at **[pulse-eight.github.io/libcec](https://pulse-eight.github.io/libcec/)**:

* [C / C++](https://pulse-eight.github.io/libcec/cpp/) — the native `ICECAdapter` interface and the C API
* [.NET](https://pulse-eight.github.io/libcec/dotnet/) — the managed `LibCecSharp` binding
* [Node.js](https://pulse-eight.github.io/libcec/nodejs/) — the N-API addon
* [Python](https://pulse-eight.github.io/libcec/python/) — the SWIG `cec` module
* [Rust](https://pulse-eight.github.io/libcec/rust/) — the `libcec` crate

The docs are generated from this source tree; see [docs/api/README.md](docs/api/README.md).

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

The upstream API surface is defined by the `LIBCEC` source tree vendored in `UPSTREAM_CLONE/` (C/C++ / CMake ecosystem). Public entry points:

- Source modules: `cmake/`, `debian/`, `include/`, `licenses/`, `project/`, `src/`, `support/`, `systemd/`
- The snapshot declares 20 dependency references across 3 ecosystem(s); see Dependencies below.
- Overlay API: `anticloud/cli.py` exposes 13 subcommands with JSON stdout; `anticloud/bench/runner.py` runs the 16-check suite; `anticloud/provenance/chain.py` exposes the SHA3-256 + Ed25519 provenance chain.

---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | C/C++ / CMake |
| Manifests detected | CMakeLists.txt |
| Files in snapshot | 286 |
| Lines of code | 54410 |
| Dependency references | 20 |
| Dependencies by ecosystem | cargo: 12, native: 6, npm: 2 |
| Upstream license | GPL-2.0 |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| cargo | name | libcec | src/rust/Cargo.toml |
| cargo | version | 8.1.7 | src/rust/Cargo.toml |
| cargo | edition | 2021 | src/rust/Cargo.toml |
| cargo | rust-version | 1.63 | src/rust/Cargo.toml |
| cargo | description | Rust binding for libCEC - control CEC-capable HDMI devices (TVs, AV receivers) via Pulse-Eight USB-CEC and SoC-native CEC | src/rust/Cargo.toml |
| cargo | homepage | https://github.com/Pulse-Eight/libcec | src/rust/Cargo.toml |
| cargo | project | https://github.com/Pulse-Eight/libcec | src/rust/Cargo.toml |
| cargo | documentation | https://pulse-eight.github.io/libcec/rust/ | src/rust/Cargo.toml |
| cargo | readme | README.md | src/rust/Cargo.toml |
| cargo | license | GPL-2.0-or-later | src/rust/Cargo.toml |
| cargo | links | cec | src/rust/Cargo.toml |
| cargo | name | libcec | src/rust/Cargo.toml |
| native | Python2 | - | src/pyCecClient/CMakeLists.txt |
| native | Python3 | - | src/pyCecClient/CMakeLists.txt |
| npm | node-addon-api | ^8.0.0 | src/nodejs/package.json |
| ... | (5 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- `CMakeLists.txt`

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

Upstream contributions: fork the `LIBCEC` project, create a feature branch, and open a pull request against upstream. Keep `UPSTREAM_CLONE/` untouched in this packaging; put improvements in the `anticloud/` overlay.

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: GPL-2.0** (evidence: `LICENSE.md` in the upstream snapshot).

License file excerpt:

```text
libCEC(R) is Copyright (C) 2011-2026 Pulse-Eight Limited.  All rights reserved.

libCEC(R) is an original work, containing original code.
libCEC(R) is a trademark of Pulse-Eight Limited.

This program is dual-licensed; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program; if not, write to the Free Software
Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA 02111-1307, USA.

Alternatively, you can license this library under a commercial license,
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original GPL-2.0 terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `GPL-2.0` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `LIBCEC` (category: CONSUMER ELECTRONICS)
- **Upstream URL:** https://github.com/bramp/libcec-daemon
- **Pinned commit (SHA):** `fe9df5ddf7356daa521f893c16872a09c8e6fb59`
- **Branch:** master
- **Pin provenance:** GitHub API commits/master. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`b1cf2d372957a8102d12025be8b1afc4c3bcd31ba64d56df915a26bde9e5fc95`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

