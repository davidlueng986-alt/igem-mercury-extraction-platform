# Mercury Detection Platform — Open Hardware

An extensible mercury-detection platform made of a water-first detection core (a mercury biosensor plus readout hardware) and pluggable extraction modules. Each module converts one kind of sample into the same standard liquid sample, so the detection core is built and validated once and a new sample type only needs a new module. Water is the simplest sample, soil is the first extraction module, and agricultural-produce and seafood modules are future work. Built by a high-school iGEM 2026 team in Hong Kong.

> **Language note:** the documents are written in Traditional Chinese; the vision document is in colloquial Cantonese.

## Documents

| Document | Description |
| --- | --- |
| [00 – Vision: a water-first platform](docs/00-vision-water-first-platform.md) | Why we propose moving from "soil only" to a water-first platform with pluggable sample modules: architecture, benefits, honest claims and roadmap (colloquial Cantonese). |
| [01 – Soil NaCl extraction module](docs/01-soil-nacl-module.md) | Hardware plan for the first extraction module (route 1): automatic weighing, NaCl dosing, stirring, settling and two-stage filtration, delivering at least 9 mL of filtrate. |
| [02 – UV-AOP oxidation module](docs/02-uv-aop-module.md) | Hardware plan for a reusable post-processing stage (UV-C LED plus dilute H₂O₂) that converts organic and complexed mercury to Hg²⁺ so the sensor can read it. |
| [03 – Water standard module](docs/03-water-module.md) | Hardware plan for the water module, the first instance of the standard interface: filtration to 0.45 µm, buffer matching and a standard liquid output of at least 9 mL. |

## Status

This project is at the **design stage**.

- The hardware has not been built yet.
- Extraction performance is predicted by modelling and has not been experimentally validated.
- The team has not performed any mercury-containing experiments.

## Safety

- The UV-AOP module uses UV-C light, which is harmful to eyes and skin, and dilute hydrogen peroxide. It must be fully enclosed with a hardware interlock (a door switch in series with the LED supply, not only a software check); see section 7 of the UV-AOP document.
- Mercury-containing samples and waste require supervised laboratory handling.

## License

The documentation is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE).
