# Order, not speed: the work price of letting go

Seth Douglas and Nidhal Mghirbi — October 2026.

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23323808.svg)](https://doi.org/10.5281/zenodo.23323808)

[Read the letter](paper/main.pdf) · [TeX source](paper/main.tex)

Landauer's principle prices erasure, and finite-time thermodynamics prices speed, a cost that patience removes.
This short letter identifies a price that patience never removes: the price of order. A device that must let
an output go before a later input arrives can no longer use that output to clean up, and it pays for every
correlation its record keeps with that output. At a fixed state, the price of releasing is the price of correlations whose partners
have left.

The letter states the principle and the work law: the optimal rate of deterministic work, over many uses at vanishing
error, for a broad class of schedules of arrivals, releases and loans (the conditions are stated in the letter), when
every borrowed system comes back with the Hamiltonian it arrived with and the device's controller comes back with its energy and entropy refunded. With the companion
results, it settles three questions:
- does answering promptly cost more? For memoryless channels, only if they are quantum;
- can one decide whether a channel is free? Yes when outputs may be held, and no when they must be released;
- what does keeping time cost? A clock that must come back supplies phase but no net energy, so in batch, thermal
  operations with a returned clock do not reach the capacity of every channel.

The price is testable: a two-qubit process that is free when held costs at least 0.87 kT ln 2 per episode
at 1% error when its first output must leave early and the controller and battery budgets total at most 0.025 (energies in kT ln 2,
entropies in bits); the error enters only through three local Pauli settings, and certifying the budgets is the remaining step.

## The series

The letter summarizes four papers, which give the full proofs and carry the machine checks.

| Paper | DOI | Repository |
|---|---|---|
| The price of time order | [10.5281/zenodo.23310622](https://doi.org/10.5281/zenodo.23310622) | [Apsiape/price-of-time-order](https://github.com/Apsiape/price-of-time-order) |
| Only quantum channels save work by waiting | [10.5281/zenodo.23310624](https://doi.org/10.5281/zenodo.23310624) | [Apsiape/save-work-by-waiting](https://github.com/Apsiape/save-work-by-waiting) |
| The work cost of answering in real time | [10.5281/zenodo.23310628](https://doi.org/10.5281/zenodo.23310628) | [Apsiape/answering-in-real-time](https://github.com/Apsiape/answering-in-real-time) |
| The price of keeping time | [10.5281/zenodo.23310632](https://doi.org/10.5281/zenodo.23310632) | [Apsiape/price-of-keeping-time](https://github.com/Apsiape/price-of-keeping-time) |

The letter cites version 1.0.2 of the first three papers by their version DOIs (10.5281/zenodo.23323043 to 23323045)
and version 1.1.0 of The price of keeping time (10.5281/zenodo.23325723); the concept DOIs above always resolve to the latest version. The papers are the authority for exact statements and hypotheses.

## Build

Requires a standard TeX distribution (TeX Live or MiKTeX) with `pdflatex`, BibTeX and the `urlbst` bibliography styles. From the
repository root, run

    python paper/build.py

The build stops on any undefined reference or citation, duplicate label or overfull box.

## How this work was done

The authors developed this work with AI models from more than one developer and take responsibility for every
claim. The last paragraph of the letter describes how the work was done, and each companion paper describes it in
full.

## License

The letter and its source are licensed under CC BY 4.0, and the build script is also available under the MIT
License; see [RIGHTS.md](RIGHTS.md) and [LICENSE](LICENSE). This is version 1.1.0 of the Zenodo record [doi:10.5281/zenodo.23323808](https://doi.org/10.5281/zenodo.23323808); that concept DOI always resolves to the latest version, and is the one to cite. Version 1.0.0 is [doi:10.5281/zenodo.23323809](https://doi.org/10.5281/zenodo.23323809). [CITATION.cff](CITATION.cff) provides machine-readable citation metadata.
