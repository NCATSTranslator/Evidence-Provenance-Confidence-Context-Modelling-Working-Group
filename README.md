# Evidence Provenance Confidence/Context (EPC) Working Group

This is the project coordination repository of the Translator *Evidence Provenance Confidence (& possibly Context) Modelling Working Group*.

## Meetings

- [WG Running Agenda](https://docs.google.com/document/d/1CsDhRYOCL1FJMDntdSNkuXZa00IXYjnyLouyLXpb8M4)
- September 2020 Relay Provenance Session ([slides](https://docs.google.com/presentation/d/1NzpnX-ZafU72mwcDt4qsRsTlT97cl0EsjzS1CqmgmbY), [notes](https://docs.google.com/document/d/1-5gj4ynmeAep1TVS7QRmEZlbBoY465Buqtju5TxEZ1E))

# Terms of Reference

- [Overview](https://docs.google.com/document/d/11HuUMw3u9uf1RPa3FbFgSgbY47hDxAFWywbCYVxUMLI)

## Requirements Gathering

- [EPC Modeling Requirements Collection](https://docs.google.com/spreadsheets/d/1WDkqNMhy7aer_3-JB4SCVhp1MZeFYZjCnYuRCnoZguo)

## Third Party Models

- July SEPIO Presentation ([slides](https://docs.google.com/presentation/d/1W_VWV5oMplK9Wz2XBXdZNLHPKcmAC3CR-3P6JwYAJMw/edit#slide=id.g7393cc5b77_0_479))

## Biolink Model Integration

For convenience of access, this project has a dedicated EPPC fork of the Biolink Model injected into this project as a Git `submodule`  in the *biolink* folder of the project.  The basic idea here is that we will make judicious EPCC revisions to this forked copy of the Biolink model,f or pull request merging into the main Biolink Model, once those changes are ready to be used by the Translator community.

## TRAPI Integration

A similar controlled EPC integration process as with the Biolink Model will likely be initiated for TRAPI as well (TBA).

## Use Cases

1. A user conducts an initial Translator ARS query which returns a non-empty knowledge graph result. They wish to view all of the available EPC information associated with a specific edge assertion in the graph, so triggers a second the ARS to retrieve all said EPC information in a second query to the graph, using some suitable edge identifier.

    a) Variant of 1: user provides specific EPCC information filters to constrain the information returned to specific types.
    b) Variant of 1 and 1a): the EPCC information returned default to 'shallow', 'breadth first', scope, so the user may ask for additional details about one or more specific components of the information returned (e.g. access details about underlying "evidence information objects" cited within the EPC).


