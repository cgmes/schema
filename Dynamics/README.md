# Dynamics Profile

The CIM dynamic model definitions reflect the most common IEEE or, in the case of wind models, IEC, representations of models as well as models included in some of the transient stability software widely used by utilities.

These dynamic models are intended to ensure interoperability between different vendors’ software products currently in use by electric utility energy companies, utilities, TSOs and RTO/ISOs.  It is important to note that each vendor is free to select its own internal implementation of these models.  Differences in vendor results, as long as they are within accepted engineering practice, caused by different internal representations, are acceptable.

![Dynamics Base](./DynamicsBase.svg)

## Standard Interconnections

This section describes the standard interconnections for various types of equipment. These interconnections are understood by the application programs and can be identified based on the presence of one of the key classes with a relationship to the static power flow model: SynchronousMachineDynamics, AsynchronousMachineDynamics, EnergyConsumerDynamics or WindTurbineType3or4Dynamics.

The relationships between classes expressed in the interconnection diagrams are intended to support dynamic behaviour described by either standard models or user-defined models.

In the interconnection diagrams, boxes which are black in colour represent function blocks whose functionality can be provided by one of many standard models or by a used-defined model. Blue boxes represent specific standard models.  A dashed box means that the function block or specific standard model is optional.

![Standard Synchronous Machine Interconnection](./StandardSynchronousMachineInterconnection.svg)

![Standard Asynchronous Machine Interconnection](./StandardAsynchronousMachineInterconnection.svg)

## Standard Models

This section contains standard dynamic model specifications grouped into packages by standard function block (type of equipment being modelled).

In the CIM, standard dynamic models are expressed by means of a class named with the standard model name and attributes reflecting each of the parameters necessary to describe the behaviour of an instance of the standard model.

## User Defined Models

This package contains user-defined dynamic model classes to support the exchange of both proprietary and explicitly defined models.

Proprietary models have behavior which, while not defined by a standard model class, is mutually understood by the sending and receiving applications based on the name passed in the .name attribute of the xxxUserDefined class.  Parameters are  passed as general attributes using as many instances of the ProprietaryParameterDynamics class as there are parameters.

Explicitly defined models describe dynamic behavior in detail in terms of control blocks and their input and output signals.

## Note

The information in this clause is reproduced from the UML with the permission of UCAIug.