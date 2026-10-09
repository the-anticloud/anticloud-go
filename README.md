# GO

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-cryptocurrency-lightgrey)

> Anticloud-hardened packaging of the upstream project `GO` in category **CRYPTOCURRENCY**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** CRYPTOCURRENCY · **Upstream:** https://github.com/golang/go · **Upstream pin:** `2f5c4cd59b43425c3074b3183ebb841ee9624cfc` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

# The Go Programming Language

Go is an open source programming language that makes it easy to build simple,
reliable, and efficient software.

![Gopher image](https://golang.org/doc/gopher/fiveyears.jpg)
*Gopher image by [Renee French][rf], licensed under [Creative Commons 4.0 Attribution license][cc4-by].*

Our canonical Git project is located at https://go.googlesource.com/go.
There is a mirror of the project at https://github.com/golang/go.

Unless otherwise noted, the Go source files are distributed under the
BSD-style license found in the LICENSE file.

### Download and Install

#### Binary Distributions

Official binary distributions are available at https://go.dev/dl/.

After downloading a binary release, visit https://go.dev/doc/install
for installation instructions.

#### Install From Source

If a binary distribution is not available for your combination of
operating system and architecture, visit
https://go.dev/doc/install/source
for source installation instructions.

### Contributing

Go is the work of thousands of contributors. We appreciate your help!

To contribute, please read the contribution guidelines at https://go.dev/doc/contribute.

Note that the Go project uses the issue tracker for bug reports and
proposals only. See https://go.dev/wiki/Questions for a list of
places to ask questions about the Go language.

[rf]: https://reneefrench.blogspot.com/
[cc4-by]: https://creativecommons.org/licenses/by/4.0/

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Unknown (no standard manifest detected)** (manifests: none detected; scanned in UPSTREAM_CLONE)
- Top-level source layout: `api/`, `doc/`, `lib/`, `misc/`, `src/`, `test/`
- Snapshot size: **14811 files**, **2392179 lines of code** (measured; see Benchmarks)
- Primary languages: `.go` (10739), `.txt` (1482), `.s` (602), `.crt` (407), `(none)` (259), `.golden` (134)
- Upstream commit pinned for this packaging: `2f5c4cd59b43425c3074b3183ebb841ee9624cfc`

---

## Installation

reliable, and efficient software.

![Gopher image](https://golang.org/doc/gopher/fiveyears.jpg)
*Gopher image by [Renee French][rf], licensed under [Creative Commons 4.0 Attribution license][cc4-by].*

Our canonical Git project is located at https://go.googlesource.com/go.
There is a mirror of the project at https://github.com/golang/go.

Unless otherwise noted, the Go source files are distributed under the
BSD-style license found in the LICENSE file.

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

No usage section was found in the upstream readme. Entry points detected in this project directory:

Browse the snapshot layout listed under What This Project Does and follow the upstream run instructions for the detected ecosystem (Unknown (no standard manifest detected)).

Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

The upstream API surface is defined by the `GO` source tree vendored in `UPSTREAM_CLONE/` (Unknown (no standard manifest detected) ecosystem). Public entry points:

- Source modules: `api/`, `doc/`, `lib/`, `misc/`, `src/`, `test/`
- The snapshot declares 78 dependency references across 1 ecosystem(s); see Dependencies below.
- Overlay API: `anticloud/cli.py` exposes 13 subcommands with JSON stdout; `anticloud/bench/runner.py` runs the 16-check suite; `anticloud/provenance/chain.py` exposes the SHA3-256 + Ed25519 provenance chain.

---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Unknown (no standard manifest detected) |
| Manifests detected | none |
| Files in snapshot | 14811 |
| Lines of code | 2392179 |
| Dependency references | 78 |
| Dependencies by ecosystem | go: 78 |
| Upstream license | BSD-3-Clause |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| go | golang.org/x/crypto | v0.57.1-0.20260921070245-7a4a4d6beae2 | src/go.mod |
| go | golang.org/x/net | v0.59.0 | src/go.mod |
| go | golang.org/x/tools | v0.50.1-0.20260929192349-98444708d405 | src/go.mod |
| go | golang.org/x/sys | v0.48.0 | src/go.mod |
| go | golang.org/x/text | v0.42.0 | src/go.mod |
| go | golang.org/x/arch | v0.26.0 | src/simd/archsimd/_gen/go.mod |
| go | golang.org/x/tools | v0.48.0 | src/simd/archsimd/_gen/go.mod |
| go | gopkg.in/yaml.v3 | v3.0.1 | src/simd/archsimd/_gen/go.mod |
| go | golang.org/x/mod | v0.38.0 | src/simd/archsimd/_gen/go.mod |
| go | golang.org/x/sync | v0.22.0 | src/simd/archsimd/_gen/go.mod |
| go | golang.org/x/tools | v0.33.0 | src/runtime/_mkmalloc/go.mod |
| go | github.com/mmcloughlin/avo | v0.6.0 | src/crypto/sha1/_asm/go.mod |
| go | golang.org/x/mod | v0.20.0 | src/crypto/sha1/_asm/go.mod |
| go | golang.org/x/sync | v0.8.0 | src/crypto/sha1/_asm/go.mod |
| go | golang.org/x/tools | v0.24.0 | src/crypto/sha1/_asm/go.mod |
| ... | (63 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- `codereview.cfg`

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

# Contributing to Go

Go is an open source project.

It is the work of hundreds of contributors. We appreciate your help!

## Before filing an issue

If you are unsure whether you have found a bug, please consider asking in the [golang-nuts mailing
list](https://groups.google.com/forum/#!forum/golang-nuts) or [other forums](https://golang.org/help/) first. If
the behavior you are seeing is confirmed as a bug or issue, it can easily be re-raised in the issue tracker.

## Filing issues

Sensitive security-related issues should be reported to [security@golang.org](mailto:security@golang.org).
See the [security policy](https://golang.org/security) for details.

The recommended way to file an issue is by running `go bug`.
Otherwise, when filing an issue, make sure to answer these five questions:

1. What version of Go are you using (`go version`)?
2. What operating system and processor architecture are you using?
3. What did you do?
4. What did you expect to see?
5. What did you see instead?

For change proposals, see [Proposing Changes To Go](https://go.dev/s/proposal-process).

## Contributing code

Please read the [Contribution Guidelines](https://golang.org/doc/contribute.html) before sending patches.

Unless otherwise noted, the Go source files are distributed under
the BSD-style license found in the LICENSE file.

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: BSD-3-Clause** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text
Copyright 2009 The Go Authors.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are
met:

   * Redistributions of source code must retain the above copyright
notice, this list of conditions and the following disclaimer.
   * Redistributions in binary form must reproduce the above
copyright notice, this list of conditions and the following disclaimer
in the documentation and/or other materials provided with the
distribution.
   * Neither the name of Google LLC nor the names of its
contributors may be used to endorse or promote products derived from
this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original BSD-3-Clause terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `BSD-3-Clause` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `GO` (category: CRYPTOCURRENCY)
- **Upstream URL:** https://github.com/golang/go
- **Pinned commit (SHA):** `2f5c4cd59b43425c3074b3183ebb841ee9624cfc`
- **Branch:** master
- **Pin provenance:** GitHub API commits/master. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`59476423d1f093887131b5fb0b6bb42280129abd518feda2ed5649fd3b722237`.

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
| DANS (KNAW/NWO, Netherlands) | 10.17026/PT | EU-recognised archive |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe
and Mail, Business Insider, National Post, Financial Post, StreetInsider,
Digital Journal, Barchart, International Business Times, and Fox News.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

