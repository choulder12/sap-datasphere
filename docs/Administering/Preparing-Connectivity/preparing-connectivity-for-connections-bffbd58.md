<!-- loiobffbd58c15784a62af0520f171018ded -->

# Preparing Connectivity for Connections

You need to perform some preparatory steps to be able to create and use connections in SAP Datasphere. The steps depend on the source you want to connect to and on the features you want to use with the connection.



The following overview lists the most common prerequisites per connection type and points to further information about what needs to be prepared to connect and use a connection.

** **


<table>
<tr>
<th valign="top">

Connection Type



</th>
<th valign="top">

Remote Tables: Data Provisioning Agent Required?



</th>
<th valign="top">

Remote Tables: Installation of Third-Party JDBC Library Required?



</th>
<th valign="top">

Data Flows and Replication Flows: Cloud Connector Required for On-Premise Sources?



</th>
<th valign="top">

Data Flows: Third-Party Driver Upload Required?



</th>
<th valign="top">

SAP Datasphere IP Required in Source Allowlist?



</th>
<th valign="top">

Server Certificate Upload Required?



</th>
<th valign="top">

Source IP Required in SAP Datasphere IP Allowlist?



</th>
<th valign="top">

Additional Information and Prerequisites



</th>
</tr>
<tr>
<td valign="top">

[Adverity](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/63e9ff5825384a03979666dbc3e715f2.html "Extend connectivity beyond SAP Datasphere standard remote connectivity and cover additional data sources that are available with Adverity.") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

yes



</td>
<td valign="top">

[Prepare Connectivity to Adverity](prepare-connectivity-to-adverity-a37a758.md)



</td>
</tr>
<tr>
<td valign="top">

[Amazon Athena](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/1b21cd00fa9842f5ba747047b80fe3ab.html "Use the connection to access data from Amazon Athena, an interactive query service which can be used to analyze data in Amazon S3 using standard SQL.") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to Amazon Athena](prepare-connectivity-to-amazon-athena-8d80f60.md)



</td>
</tr>
<tr>
<td valign="top">

[Amazon Redshift](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/8b132061d4e149d9a16b3576dda1f613.html "Use the connection to access data from Amazon Redshift 8.x databases.") :arrow_upper_right:



</td>
<td valign="top">

yes



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

yes



</td>
<td valign="top">

yes \(Outbound IP Address\)



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to Amazon Redshift](prepare-connectivity-to-amazon-redshift-519b2db.md)



</td>
</tr>
<tr>
<td valign="top">

[Amazon Simple Storage Service](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/a7b660a0a4ef4a4fbee57b44f5b2147d.html "Use the connection to access data from objects in Amazon S3.") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

n/a



</td>
</tr>
<tr>
<td valign="top">

[Cloud Data Integration](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/cd33107246f446628f9baff56faf5a1b.html "Use the connection to access data from SAP cloud applications which provide OData-based APIs for data integration and have a Cloud Data Integration (CDI) provider service implemented.") :arrow_upper_right:



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

yes \(for data flows\)



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity for Cloud Data Integration](prepare-connectivity-for-cloud-data-integration-b6fd8de.md)



</td>
</tr>
<tr>
<td valign="top">

[Generic JDBC](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/eeae3aca6d0040149f7b1e658c434f15.html "Use the connection to access data from tables and views in any supported data source for which a JDBC driver is available.") :arrow_upper_right:



</td>
<td valign="top">

yes \(for on-premise\)



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity for Generic JDBC](prepare-connectivity-for-generic-jdbc-648fabf.md)



</td>
</tr>
<tr>
<td valign="top">

[Generic OData](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/5d36f1aae68a4e59989c424a66d948c9.html "Use the connection to access data from an OData service.") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

yes \(for data flows\)



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity for Generic OData](prepare-connectivity-for-generic-odata-d9c43a2.md)



</td>
</tr>
<tr>
<td valign="top">

[Generic SFTP](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/b645de78a8374c24871ab6169be40d35.html "Use the connection to access files on a Secure File Transfer Protocol (SFTP) server.") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity for Generic SFTP](prepare-connectivity-for-generic-sftp-5454a8c.md)



</td>
</tr>
<tr>
<td valign="top">

[Google BigQuery](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/30ed77de13864368bdc596099b37ed70.html "Use the connection to access data from a Google BigQuery data source..") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to Google BigQuery](prepare-connectivity-to-google-bigquery-529cef1.md)



</td>
</tr>
<tr>
<td valign="top">

[Google Cloud Storage](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/aec242c29188408c9ebe1a3ab63ce28b.html "Use the connection to access objects from Google Cloud Storage.") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

n/a



</td>
</tr>
<tr>
<td valign="top">

[Hadoop Distributed File System](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/f9c33566c4eb412d9d36a2f044bb5126.html "Use the connection to access objects from an Hadoop Distributed File System (HDFS) server.") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

n/a



</td>
</tr>
<tr>
<td valign="top">

[Microsoft Azure Blob Storage](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/df5a7c56ac21472c973f6fab341f3991.html "Use the connection to access objects in Microsoft Azure Blob Storage.") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

n/a



</td>
</tr>
<tr>
<td valign="top">

[Microsoft Azure Data Lake Store Gen1](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/aa04f9a3dd454b1b8761a963079887a3.html "Use the connection to access objects in Microsoft Azure Data Lake Gen1 (ADL Gen1).") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

n/a



</td>
</tr>
<tr>
<td valign="top">

[Microsoft Azure Data Lake Store Gen2](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/cd06b3c5ab5147c0905e3fa8abd13eb1.html "Use the connection to access objects in Microsoft Azure Data Lake Gen2 (ADL Gen2).") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

n/a



</td>
</tr>
<tr>
<td valign="top">

[Microsoft Azure SQL Database](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/46343fc1c4544fa9a075d97f84d39826.html "Use the connection to access table data from a Microsoft Azure SQL database.") :arrow_upper_right:



</td>
<td valign="top">

yes



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

yes \(Outbound IP Address\)



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to Microsoft Azure SQL Database](prepare-connectivity-to-microsoft-azure-sql-database-782bd8c.md)



</td>
</tr>
<tr>
<td valign="top">

[Microsoft SQL Server](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/a13c8abb328f45be891599c9cc76fb91.html "Use the connection to access data from a Microsoft SQL Server (on-premise).") :arrow_upper_right:



</td>
<td valign="top">

yes



</td>
<td valign="top">

yes



</td>
<td valign="top">

yes \(for data flows\)



</td>
<td valign="top">

no \(pre-bundled; no upload required\)



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to Microsoft SQL Server](prepare-connectivity-to-microsoft-sql-server-ea69328.md)



</td>
</tr>
<tr>
<td valign="top">

[Open Connectors](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/9bfe7db51216449d985a0b59f5e181c4.html "Use the connection to access data from sources that are connected to the SAP Open Connectors account that is integrated with your space.") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to SAP Open Connectors](prepare-connectivity-to-sap-open-connectors-fb1aa11.md)



</td>
</tr>
<tr>
<td valign="top">

[Oracle](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/c73ae0601d364f47830d339b6e86b7e8.html "Use the connection to access data from an Oracle database (on-premise).") :arrow_upper_right:



</td>
<td valign="top">

yes



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to Oracle](prepare-connectivity-to-oracle-9fca7c4.md)



</td>
</tr>
<tr>
<td valign="top">

[Precog](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/6e5f2255ae8540d5895dcbef4157b82d.html "Extend connectivity beyond SAP Datasphere standard remote connectivity and cover additional data sources that are available with Precog.") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

yes



</td>
<td valign="top">

[Prepare Connectivity to Precog](prepare-connectivity-to-precog-ad13c31.md)



</td>
</tr>
<tr>
<td valign="top">

[SAP ABAP](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/a75c1aacf951449ba3b740c7e46da3a9.html "Use the connection to access data from SAP ABAP on-premise systems through RFC or to access data from cloud source systems such as SAP S/4HANA Cloud through Web Socket RFC.") :arrow_upper_right:



</td>
<td valign="top">

yes \(for on-premise\)



</td>
<td valign="top">

no



</td>
<td valign="top">

yes \(for on-premise: for data flows and replication flows\)



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to SAP ABAP Systems](prepare-connectivity-to-sap-abap-systems-76c9ac1.md)



</td>
</tr>
<tr>
<td valign="top">

[SAP BW](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/e589041e80264f43b6c209c407336376.html "Use the connection to access data from virtual tables through RFC for ODP sources (extractors) and ABAP Dictionary tables from SAP Business Warehouse (SAP BW) or SAP BW∕4HANA systems. For SAP BW systems that don&apos;t have the ABAP Pipeline Engine extension installed, ODP extractors can be used as sources in data flows.") :arrow_upper_right:



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

yes \(for data flows\)



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to SAP BW](prepare-connectivity-to-sap-bw-b0b371e.md)



</td>
</tr>
<tr>
<td valign="top">

[SAP BW∕4HANA Model Transfer](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/1caba954bc604e00bf8e82e383a46368.html "Use the connection to import analytic queries from SAP BW∕4HANA with their Composite Providers and InfoObjects.") :arrow_upper_right:



</td>
<td valign="top">

yes \(to connect to the SAP HANA database of SAP BW/4HANA\)



</td>
<td valign="top">

no



</td>
<td valign="top">

yes \(to make http requests to SAP BW/4HANA\)



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Preparing SAP BW/4HANA Model Transfer Connectivity](preparing-sap-bw-4hana-model-transfer-connectivity-962de2f.md)



</td>
</tr>
<tr>
<td valign="top">

[SAP ECC](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/e546ccd61af54bf49a0f531a43fe0961.html "Use the connection to access data from virtual tables through RFC for ODP sources (extractors) and ABAP Dictionary tables from SAP ECC systems (on-premise). For source systems that don&apos;t have the ABAP Pipeline Engine extension installed, ODP extractors can be used as sources in data flows.") :arrow_upper_right:



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

yes \(for data flows\)



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to SAP ECC](prepare-connectivity-to-sap-ecc-cfc1b48.md)



</td>
</tr>
<tr>
<td valign="top">

[SAP Fieldglass](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/bda94ee6c9d5403f8556af174399d221.html "Retrieves data from SAP Fieldglass. The connection type supports view building and remote tables as well as data flows.") :arrow_upper_right:



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

yes \(for data flows\)



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to SAP Fieldglass](prepare-connectivity-to-sap-fieldglass-03ca236.md)



</td>
</tr>
<tr>
<td valign="top">

[SAP HANA](https://help.sap.com/viewer/be5967d099974c69b77f4549425ca4c0/cloud/en-US/e6b63f176d3640609adcf06297fb37e9.html#loioe6b63f176d3640609adcf06297fb37e9 "Use the connection to access data from a remote SAP HANA database (on-premise or cloud).") :arrow_upper_right:



</td>
<td valign="top">

yes \(for on-premise\)



</td>
<td valign="top">

no



</td>
<td valign="top">

yes \(for on-premise: for data flows and replication flows, or when using Cloud Connector for remote tables feature\)



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

yes \(for cloud\)



</td>
<td valign="top">

Cloud Connector IP \(for on-premise when using Cloud Connector for remote tables feature\)



</td>
<td valign="top">

[Prepare Connectivity to SAP HANA](prepare-connectivity-to-sap-hana-d7f22cf.md)



</td>
</tr>
<tr>
<td valign="top">

[SAP HANA Cloud, Data Lake Files](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/356e41e880e54255891b702d2afefeb3.html "Use the connection to access data from the Files component of a standalone SAP HANA Cloud, data lake.") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
</tr>
<tr>
<td valign="top">

[SAP HANA Cloud, Data Lake Relational Engine](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/40763e2e3e33440db0c37f6bcbe650f0.html "Use the connection to access table data from the Relational Engine component of a standalone SAP HANA Cloud, data lake.") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

n/a



</td>
</tr>
<tr>
<td valign="top">

[SAP Marketing Cloud](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/4de4959620c24d12a53a3cc357d3e003.html "Use the connection to access data from SAP Marketing Cloud via its OData-based APIs for data integration and SAP HANA Smart Data Integration.") :arrow_upper_right:



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

yes \(for data flows\)



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to SAP Marketing Cloud](prepare-connectivity-to-sap-marketing-cloud-f5e0c06.md)



</td>
</tr>
<tr>
<td valign="top">

[SAP SuccessFactors](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/39df02030d4b411487bacecf9afea4e8.html "Use the connection to access employee-related data in SAP SuccessFactors.") :arrow_upper_right:



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

yes \(HANA IP Address\)



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to SAP SuccessFactors](prepare-connectivity-to-sap-successfactors-c9b1915.md)



</td>
</tr>
<tr>
<td valign="top">

[SAP S/4HANA Cloud](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/a98e5ffdf47c44d9a845dca01a18bd82.html "Use the connection to access or import extraction-enabled ABAP Core Data Services views (ABAP CDS views) from SAP S/4HANA Cloud.") :arrow_upper_right:



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to SAP S/4HANA Cloud](prepare-connectivity-to-sap-s-4hana-cloud-abb159e.md)



</td>
</tr>
<tr>
<td valign="top">

[SAP S/4HANA On-Premise](https://help.sap.com/viewer/9f36ca35bc6145e4acdef6b4d852d560/internal/en-US/a49a1e3cc50f4af89711d8306bdd8f26.html "Use the connection to access data from SAP S/4HANA on-premise systems.") :arrow_upper_right:



</td>
<td valign="top">

yes



</td>
<td valign="top">

no



</td>
<td valign="top">

yes \(for data flows and replication flows\)



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

no



</td>
<td valign="top">

[Prepare Connectivity to SAP S/4HANA On-Premise](prepare-connectivity-to-sap-s-4hana-on-premise-8de01dd.md)



</td>
</tr>
</table>

> ### Note:  
> For information about supported versions of sources that are connected via SAP HANA smart data integration and its Data Provsioning Agent, see the [SAP HANA smart data integration and all its patches Product Availability Matrix \(PAM\) for SAP HANA SDI 2.0](https://support.sap.com/content/dam/launchpad/en_us/pam/pam-essentials/TIP/PAM_HANA_SDI_2_0.pdf).
> 
> For information about necessary JDBC libraries for connecting to sources from third-party vendors, see:
> 
> -   [SAP HANA smart data integration and all its patches Product Availability Matrix \(PAM\) for SAP HANA SDI 2.0](https://support.sap.com/content/dam/launchpad/en_us/pam/pam-essentials/TIP/PAM_HANA_SDI_2_0.pdf)
> 
> -   [Register Adapters with SAP Datasphere](register-adapters-with-sap-datasphere-085fc49.md)

