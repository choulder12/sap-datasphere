<!-- loio3de55a78a4614deda589633baea28645 -->

# Integrating Data via Database Users/Open SQL Schemas

Create a database user in your space to read and write directly to the SAP HANA Cloud database on which SAP Datasphere runs. Each database user has an Open SQL schema, which is attached to a space schema and provides a secure method for exchanging data with the space.

Depending on the privileges they are granted, a database user can use their Open SQL schema to:

-   Create tables and views and write data to them \(see [Connect to Your Open SQL Schema](connect-to-your-open-sql-schema-b78ad20.md)\). Space members can use these objects as sources when creating views and data flows \(see [Using the Source Browser](https://help.sap.com/viewer/24f836070a704022a40c15442163e5cf/internal/en-US/7d2b21d974e44bdc9d548cf7532b5a43.html "You use the Source Browser to add objects as sources for your data flow, graphical view, SQL view, or intelligent lookup. In an E/R model you add objects to visualize them together in a diagram, including importing objects from connections and other sources, and prepare them for use in other editors.") :arrow_upper_right:\).

    ![Open SQL Schema Objects are Sources for Space](images/Open_SQL_as_Source_6401fe8.png)

-   Access the space schema and read data from the space.

    ![Open SQL Schema Reads View Exposed for Consumption](images/Open_SQL_Read_Exposed_View_a9a83fe.png)

    > ### Note:  
    > Database users can only read data from views that are created in the space with which they are associated if the view has the *Expose for Consumption* property enabled \(see [Exposing a View For Consumption](https://help.sap.com/viewer/24f836070a704022a40c15442163e5cf/internal/en-US/40ec77ec24f244279a81448969a7e769.html "To make a view available for consumption in SAP Analytics Cloud and other clients, tools, and apps (including via the public ODATA API), enable the Expose for Consumption switch.") :arrow_upper_right:\).

-   Create a table to act as a target to receive data written from a data flow \(see [Allow the Space to Write to the Open SQL Schema](allow-the-space-to-write-to-the-open-sql-schema-7eaa370.md)\).

    ![Space Data Flow Writes to Open SQL Schema Table](images/Open_SQL_Write_from_Space_1a84b15.png)


A database user is required in order to:

-   Connect an analytics client or other tool to SAP Datasphere \(see [Consume Data in Power BI and Other Third-Party Clients, Tools, and Apps](https://help.sap.com/viewer/24f836070a704022a40c15442163e5cf/internal/en-US/add771abf6f54c9d8de4c7e470a0e6f0.html "You can consume data exposed as views in Microsoft Power BI and other third-party clients, tools, and apps. You can connect to SAP Datasphere through the OData API, or via an Open SQL schema.") :arrow_upper_right:\).
-   Consume space data in an SAP SQL Data Warehousing HDI container \(see [Access Space Objects in Your HDI Container](../../Exchanging-Data-with-SAP-SQL-Data-Warehousing-HDI-Container/access-space-objects-in-your-hdi-container-656eebc.md)\).
-   Work with SAP HANA Cloud, data lake \(see [Integrating Data to and From SAP HANA Cloud Data Lake](../../Integrating-Data-to-and-From-HANA-Cloud/integrating-data-to-and-from-sap-hana-cloud-data-lake-e84545b.md)\).

> ### Note:  
> Users with the DW Administrator role can create database user groups, which are similar to database users, but which are not assigned to a single space and can allow multiple spaces to read from and write to their schemas \(see [Creating Database User Groups](https://help.sap.com/viewer/935116dd7c324355803d4b85809cec97/internal/en-US/1097a470be40432e89f91288bdc14378.html "Create database user groups with corresponding administrators that can directly connect to the the underlying SAP HANA Cloud database and work with SQL.") :arrow_upper_right:\).

