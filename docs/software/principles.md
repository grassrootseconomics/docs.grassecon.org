# System Design Principles

The guiding principles for system design and contribution are described below with emphasis on software development and infrastructure.


## Massively scalable

The queueing and syncing engine should be able to queue and sync state change requests and state queries to the full capacity of the integrated networks, without any loss of data and with minimum middleware latency for the end-user.

## Avoid lock-ins

.. whether by opacity, complexity or license terms.

No part of the system should rely on and/or integrate with libraries or services that cannot be reasonably understood and/or adapted.

Nor should the work required to replace a component be unreasonable large as a result of external dependencies.

It should also be straightforward for services implementers to choose their own services dependencies (like chains, chain nodes, SaaS deferrals etc).


## Lean dependency graph

The base components should make use of primitives and standard libraries as much as possible.

The services components written for Grassroots Economics specifically should only rely on generic base components.


## Network state as the source of truth

Changes to state is sent to network immediately.

State queries made through the engine always retrieve state from network before being adjusted.


## Split engine into reusable modules

Which in essence is practical implementation of the "system parts" chapter below.


## No soft lock-in to virtual environments

Too many modern software projects only provides reasonable ease of use through mechanisms like Docker or similar frameworks.

Care should be taken to incur minimum penalty for using the application and tooling in a local host environment.

Documentation must exist and be maintained to facilitate this.

Furthermore, there should exist local-only alternate services of the underlying base components. Example of this is the [chaind](https://gitlab.com/chaintool/chaind) / [chaind-eth](https://gitlab.com/chaintool/chaind-eth) pair which enables queue/sync dynamics in a local services (e.g. systemd) environment for an independent wallet.


## Coherent configurations regardless of entry-point

Merged ini-format configuration files constitute configuration schemas and overrides, translating to a configuration directive vocabulary overridable by environment variables of the same name.


## CLI tooling framework

Layered definitions of command line arguments, so that concepts common for each layer is only defined in one place.

Full and intuitive control of overriding configuration directives with command line arguments and flags.

Easy generation of base resource objects (such as rpc, wallet) directly from rendered configurations.

Facilitate and encourage use of chainable commands (e.g. UNIX pipelines).
