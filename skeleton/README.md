# ${{values.name | dump}}

- [Overview](#overview)
- [Usage](#usage)

## Overview

Use this component to create a Data Product.

A Data Product by itself does not provision any resources or infrastructure (components contained within it usually do), and as such this Template can be used without any Specific Provisioner.

### What's a Template?

A Template is a tool that helps create components inside a Data Mesh. Templates help establish a standard across the organization. This standard leads to easier understanding, management and maintenance of components. Templates provide a predefined structure so that developers don't have to start from scratch each time, which leads to faster development and allows them to focus on other aspects, such as testing and business logic.

For more information, please refer to the [official documentation](https://docs.witboost.agilelab.it/docs/p1_user/p6_advanced/p6_1_templates/#getting-started).

### What's a Data Product?

A data product is a logical unit that contains all components to process and store domain data for analytical or data-intensive use cases and makes them available to other teams via output ports. You can think of a microservice, but for analytical data.

Data products connect to sources, such as operational systems or other data products and perform data transformation. Data products serve data sets in one or many output ports.

A data product is owned by a domain team. The team is responsible for the operations of the data product during its entire lifecycle.

## Usage

To get information on how to use this template, refer to this [document](docs/index.md).