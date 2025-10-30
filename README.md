# eof-eos-stac-extension

- **Title:** Framework for Earth Observation Science Missions
- **Identifier:** <https://xxx.github.io/eof-eos-stac-extension/v0.1.0/schema.json>
- **Field Name Prefix:** eof-eos
- **Scope:** Item
- **Extension [Maturity Classification](https://github.com/radiantearth/stac-spec/tree/master/extensions/README.md#extension-maturity):** Proposal
- **Owner**: European Space Agency
- **History:** Proposal in preparation

This document explains the fields of the EOF-EOS extension to the
[SpatioTemporal Asset Catalog](https://github.com/radiantearth/stac-spec) (STAC) specification.

EOF-EOS is ESA Missions, Data and Operations Management Framework for EO Science Missions.
See the EOF-EOS Web site for context.

It is strongly recommended to use the other STAC extensions eo, view, processing, sat and sci with the eof-eos extension.

- Examples:
  - [Item example](examples/item.json)
- [JSON Schema](json-schema/schema.json)
- [Changelog](./CHANGELOG.md)

## Item Properties



| Field Name               | Type                                                   | Description                      |
| ------------------------ | ------------------------------------------------------ | -------------------------------- |
| eof-eos:global_coverage_id       | string                                                  | Global coverage identifier.  |
| eof-eos:is_coregistration_primary     | boolean                                               | Is coregistration primary. Example: true.     |
| eof-eos:major_cycle_id       | string                                                 | Major cycle identifier.  |
| eof-eos:mission_phase       | string                                                 | Mission phase. Example: "COMMISSIONING". |
| eof-eos:orbit_drift_flag       | boolean                                                 | Orbit drift flag. Example: false.  |
| eof-eos:repeat_cycle_id       | string                                                 | Repeat cycle identifier.  |
| eof-eos:stack_id     | string                                                 | Stack identifier. Example "BIO_S1_STA__ID_20250606T094957_20250621T095020_C_G___M___S0276_W0562_A_01_DGMWJZ". |


## Contributing

All contributions are subject to the
[STAC Specification Code of Conduct](https://github.com/radiantearth/stac-spec/blob/master/CODE_OF_CONDUCT.md).
For contributions, please follow the
[STAC specification contributing guide](https://github.com/radiantearth/stac-spec/blob/master/CONTRIBUTING.md) Instructions
for running tests are copied here for convenience.

### Running tests

The same checks that run as checks on PR's are part of the repository and can be run locally to verify that changes are valid. 
To run tests locally, you'll need `npm`, which is a standard part of any [node.js installation](https://nodejs.org/en/download/).

First you'll need to install everything with npm once. Just navigate to the root of this repository and on 
your command line run:
```bash
npm install
```

Then to check markdown formatting and test the examples against the JSON schema, you can run:
```bash
npm test
```

This will spit out the same texts that you see online, and you can then go and fix your markdown or examples.

If the tests reveal formatting problems with the examples, you can fix them with:
```bash
npm run format-examples
```




