# OpenChain Project Landscape

![OpenChain Landscape Logo](https://openchainproject.org/wp-content/uploads/sites/30/2019/10/openchain-hztl-color-01.svg)

This landscape is intended as a map to explore open source projects hosted by the OpenChain Project and also shows its member companies. It is modeled after the Cloud Native Computing Foundation (CNCF) [landscape](https://landscape.cncf.io) and based on the same open-source code.

This repository contains the data files and images required to generate the [OpenChain Project landscape](https://landscape.openchainproject.org). The software that generates it can be found at the [cncf/landscape2](https://github.com/cncf/landscape2) repository. Please see its [README file](https://github.com/cncf/landscape2#landscape2) for more information about how it works.

## New Entries and Corrections

OpenChain Conformance and Partner Program data ( which in the [landscape.yml](landscape.yml) file are under the categories `Conformance` and `Partner` ) are created and managed by the OpenChain Staff.

- If you see errors with entries in these two categories, you either open a pull request with edits to [landscape.yml](landscape.yml), or [create a helpdesk ticket](https://members.linuxfoundation.org) to request those changes.

OpenChain Project Member data in this repository ( which in the [landscape.yml](landscape.yml) file are under category `Member` ) are built nightly using the [LFX Landscape Tools](https://github.com/jmertic/lfx-landscape-tools). Any changes made directly in the data files in this repository for the above-referenced categories will be overwritten.

- For `Member` entries, you can either make these changes in [LFX Organization Dashboard](https://docs.linuxfoundation.org/lfx/organization-dashboard/organization-profile) or [create a helpdesk ticket](https://members.linuxfoundation.org) to request those changes.

If the error is with data from [Crunchbase](https://www.crunchbase.com/) you should open an account there and edit the data. 

## Local Build and Install

You can build the landscape locally on your machine using the [landscape2](https://github.com/cncf/landscape2) tool. Once [installed](https://github.com/cncf/landscape2?tab=readme-ov-file#installation), you can use the commands below to build the landscape and serve it locally.

```shell
landscape2 build --data-file landscape.yml --settings-url https://raw.githubusercontent.com/cncf/landscape2-sites/refs/heads/main/openchain/settings.yml --logos-path hosted_logos --output-dir build
landscape2 serve --landscape-dir build
```

## License

The generated landscape contains data received from [Crunchbase](http://www.crunchbase.com). This data is not licensed pursuant to the [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0.txt). It is subject to Crunchbase’s Data Access Terms, available at [https://data.crunchbase.com/docs/terms](https://data.crunchbase.com/docs/terms), and is only permitted to be used with OpenChain Project landscape projects.

Everything else is under the [Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0.txt), except for projects and products logos, which are generally copyrighted by the company that created them, and are simply cached here for reliability. The generated landscape and the [landscape.yml](landscape.yml) file are alternatively available under the [Creative Commons Attribution 4.0 license](https://creativecommons.org/licenses/by/4.0/).
