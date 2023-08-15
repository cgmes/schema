# Common Grid Model Exchange Specification

Profiles for the Common Grid Model Exchange Specification (CGMES).

## Introduction

The CGMES profiles are defined using non-standard UML with a closed source, Windows only desktop application with limited export functionality.
The profiles are [provided by ENTSO-E](https://www.entsoe.eu/news/2022/10/19/cgmes-3-0-publishing/) in an opaque, proprietary format.
This project aims to make the profiles more readily accessible by distributing
them in standardized formats, serialized in well estabished syntaxes.

The profiles are exported as UML v1.3 in XMI v1.1 format.
The UML is converted to [RDFS](https://www.w3.org/TR/rdf-schema/) in [RDF/XML](https://www.w3.org/TR/rdf-syntax-grammar/), [Turtle](https://www.w3.org/TR/turtle/) and [N-Triples](https://www.w3.org/TR/n-triples/) format.

## Profiles

### Part 452

 - [Core Equipment](./CoreEquipment/README.md)
 - [Short Circuit](./ShortCircuit/README.md)
 - [Operation](./Operation/README.md)

### Part 456

 - [Topology](./Topology/README.md)
 - [Steady State Hypothesis](./SteadyStateHypothesis/README.md)
 - [State Variables](./StateVariables/README.md)

### Part 457

 - [Dynamics](./Dynamics/README.md)
 - [Detailed Model Configuration](./DetailedModelConfiguration/README.md)
 - [Detailed Model Parameterization](./DetailedModelParameterization/README.md)
 - [Simulation Results](./SimulationResults/README.md)
 - [Simulation Settings](./SimulationSettings/README.md)

### Part 453

 - [Diagram Layout](./DiagramLayout/README.md)

### Part 13

 - [Geographical Location](./GeographicalLocation/README.md)

### Deprecated

 - [Equipment Boundary](./EquipmentBoundary/README.md)

### Metadata

 - [Document Header](./DocumentHeader/README.md)


## Legal

Licensed under either the Apache License, Version 2.0 ([LICENSE](LICENSE) or https://www.apache.org/licenses/LICENSE-2.0).

NB: This is is an unofficial source for the CGMES profiles.
Please refer to the [ENTSO-E](https://www.entsoe.eu) website for official resources.