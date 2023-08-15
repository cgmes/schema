# Equipment Profile

- UML: [[XMI]](./CoreEquipment.xmi)
- RDFS: [[Turtle]](./CoreEquipment.ttl) [[RDF/XML]](./CoreEquipment.rdf) [[N-Triples]](./CoreEquipment.nt)
- CSV: [[Class]](./CoreEquipmentClass.csv) [[Property]](./CoreEquipmentProperty.csv)

This profile has been built on the basis of the IEC 61970-452 document and adjusted to fit the purpose of the ENTSO-E CGMES.

## Core

Contains the core `PowerSystemResource` and `ConductingEquipment` entities shared by all applications plus common collections of those entities. Not all applications require all the Core entities.  This package does not depend on any other package except the Domain package, but most of the other packages have associations and generalizations that depend on it.

![Main](./Main.svg)

## Wires

An extension to the Core and Topology package that models information on the electrical characteristics of Transmission and Distribution networks. This package is used by network applications such as State Estimation, Load Flow and Optimal Power Flow.

![Wires](./Wires.svg)

## Production

The production package is responsible for classes which describe various kinds of generators. These classes also provide production costing information which is used to economically allocate demand among committed units and calculate reserve quantities.

![Production](./Production.svg)

## Load Model

This package is responsible for modeling the energy consumers and the system load as curves and associated curve data. Special circumstances that may affect the load, such as seasons and daytypes, are also included here.

This information is used by Load Forecasting and Load Management.

![Load Model](./LoadModel.svg)