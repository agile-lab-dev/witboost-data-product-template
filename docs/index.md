### Prerequisites

A Domain should already exist in order to place the newly created Data Product into it.


### Component Basic Information

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


After this the system will show you the summary of the template, and you can go back and edit or go ahead and create the Component. With the examples values given here it should look something like this:

After clicking on "Create" the registration of the Data product will start. If no errors occurred it will go through the 3 phases (Fetching, Publishing and Registering) and will give you the links to the newly created Repository and the data product page in the Builder.