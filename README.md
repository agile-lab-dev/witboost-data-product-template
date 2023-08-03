<p align="center">
    <a href="https://www.agilelab.it/witboost">
        <img src="docs/img/witboost_logo.svg" alt="witboost" width=600 >
    </a>
</p>

Designed by [Agile Lab](https://www.agilelab.it/), witboost is a versatile platform that addresses a wide range of sophisticated data engineering challenges. It enables businesses to discover, enhance, and productize their data, fostering the creation of automated data platforms that adhere to the highest standards of data governance. Want to know more about witboost? Check it out [here](https://www.agilelab.it/witboost) or [contact us!](https://www.agilelab.it/contacts)

This repository is part of our [Starter Kit](https://github.com/agile-lab-dev/witboost-starter-kit) meant to showcase witboost's integration capabilities and provide a "batteries-included" product.

# Data Product Template

- [Overview](#overview)
- [Usage](#usage)

## Overview

Use this template to create a Data Product.

A Data Product by itself does not provision any resources or infrastructure (components contained within it usually do), and as such this Template can be used without any Specific Provisioner.

### What's a Template?

A Template is a tool that helps create components inside a Data Mesh. Templates help establish a standard across the organization. This standard leads to easier understanding, management and maintenance of components. Templates provide a predefined structure so that developers don't have to start from scratch each time, which leads to faster development and allows them to focus on other aspects, such as testing and business logic.

For more information, please refer to the [official documentation](https://docs.witboost.agilelab.it/docs/p1_user/p6_advanced/p6_1_templates/#getting-started).

## Usage

### Prerequisites

A Domain should already exist in order to place the newly created Data Product into it.

### Component basic information

In the **Data Product details** section, you are expected to provide some basic information related to the Data Product. The description of each field is provided below and after that you will also find an example to better understand what values you can use to create your first Data Product:

- Name: Name of the Data Product that will be displayed after the creation.
- Domain: Domain in which we want to create the Data Product (Required). In our sandbox environment, you will find the following domains: demographic, economic_impact and healthcare.
- Identifier: A unique **uneditable** identifier for the entity inside the domain, that will be generated automatically according to the Data Product name provided and the Domain selected. It also contains a number representing the major version of it.
- Fully Qualified Name: Human-readable name that uniquely identifies an entity. You can copy it from the above `name` field (or) add more details to it (Optional).
- Description: Detailed description about what functional area this DP is representing, what is its purpose, and other business related information (Required).
- Development Group: it represents the group of developers with access to the Data Product repositories (Required). A group referring your company name and related to the accounts that we are providing to you should be already created inside the sandbox environment, so you can select it.
- Data Product Owner: The user who owns the particular Data Product (Required).
- Contact email: Point of contact, it could be the owner or a distribution list (Required).
- Information SLA: Describe what SLA the DP team is providing to answer additional information requests about the Data Product (Optional).
- Maturity: Choosing whether this Data Product is tactically created (or) not. Could be really useful during migration from DWH or Data Lake (Optional).

_Example:_

| Field name             | Example value                       |
|:-----------------------|:------------------------------------|
| **Name**               | Vaccinations                        |
| **Domain**             | domain:healthcare                   |
| **_Identifier_**       | _healthcare.vaccinations.0_         |
| **Description**        | Full history of COVID vaccinations  |
| **Development Group**  | _group:datameshplatform_            |
| **Data Product**       | system:healthcare.vaccinations.0    |
| **Data Product Owner** | user:joe.smith_mycompany.com        |
| **Contact Email**      | joe.smith@mycompany.com             |
| **Information SLA**    | Example SLA                         |
| **Maturity**           | Tactical                            |

### Choose a location

Every component needs a host where the generated code will be saved. The default is `gitlab.com`. Refer to your team to understand the structure on how to use your repository to save the components.

- Host: The host where the repository will be created. By default is `gitlab.com`
- User/Group: A group or a user that the repository belongs to, e.g. 'group/sub-group/sub-sub-group' or 'name.surname'. There are two ways of creating a new component. One way of creating it is by making a monorepo (in that way you will never change the field 'Repository' and it will always be a repository containing your data product, and you will only need to change the root directory). The second way of creating a new component is by doing it always in another repository (in that case the root directory will always be '.' and you will always change the repository field).
- Repository: The name of the repository
- Root Directory: The path that will be used as the repository root for this component. For monorepos this will be different for each component.

*Example:*

| Field name        | Example value                                  |
|:------------------|:-----------------------------------------------|
| ***Host***        | gitlab.com                                     |
| **User/Group**    | MyCompany/mesh.repository/sandbox/vaccinations |
| **Repository**    | VaccinationsDBTComponent                       |
| **RootDirectory** | .                                              |

After this the system will show you the summary of the template, and you can go back and edit or go ahead and create the Component. With the examples values given here it should look something like this:

After clicking on "Create" the registering of the Component will start. If no errors occurred it will go through the 3 phases (Fetching, Publishing and Registering) and will give you the links to the newly created Repository and the component in the Catalog.

## License

This project is available under the [Apache License, Version 2.0](https://opensource.org/licenses/Apache-2.0); see [LICENSE](LICENSE) for full details.

## About us

<p align="center">
    <a href="https://www.agilelab.it">
        <img src="docs/img/agilelab_logo.jpg" alt="Agile Lab" width=600>
    </a>
</p>

Agile Lab creates value for its Clients in data-intensive environments through customizable solutions to establish performance driven processes, sustainable architectures, and automated platforms driven by data governance best practices.

Since 2014 we have implemented 100+ successful Elite Data Engineering initiatives and used that experience to create Witboost: a technology agnostic, modular platform, that empowers modern enterprises to discover, elevate and productize their data both in traditional environments and on fully compliant Data mesh architectures.

[Contact us](https://www.agilelab.it/contacts) or follow us on:
- [LinkedIn](https://www.linkedin.com/company/agile-lab/)
- [Instagram](https://www.instagram.com/agilelab_official/)
- [YouTube](https://www.youtube.com/channel/UCTWdhr7_4JmZIpZFhMdLzAA)
- [Twitter](https://twitter.com/agile__lab)