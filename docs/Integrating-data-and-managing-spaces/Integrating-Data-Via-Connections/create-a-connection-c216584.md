<!-- loioc2165842082c43fc85bad9f0c97572bb -->

<link rel="stylesheet" type="text/css" href="../css/sap-icons.css"/>

# Create a Connection

Create a connection to allow the members of the space to use the connected source for data modeling and data access in SAP Datasphere.



<a name="loioc2165842082c43fc85bad9f0c97572bb__prereq_uvr_xng_rlb"/>

## Prerequisites

See [Preparing Connectivity for Connections](https://help.sap.com/viewer/935116dd7c324355803d4b85809cec97/internal/en-US/bffbd58c15784a62af0520f171018ded.html "You need to perform some preparatory steps to be able to create and use connections in SAP Datasphere. The steps depend on the source you want to connect to and on the features you want to use with the connection.") :arrow_upper_right:.



## Procedure

1.  In the side navigation area, click <span class="FPA-icons"></span> \(*Connections*\), select a space if necessary, and then click the *Local Connections* tab.

2.  Click *Create* to open the connection creation wizard.

3.  Click an appropriate connection type tile for your source.

    One or more of the following options help you to quickly find the connection type you need:


    <table>
    <tr>
    <th valign="top">

    Option


    
    </th>
    <th valign="top">

    Description


    
    </th>
    </tr>
    <tr>
    <td valign="top">

    Search


    
    </td>
    <td valign="top">

    In the search field, enter a search string to only show connection types that contain the string.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    Sort


    
    </td>
    <td valign="top">

    Use <span class="SAP-icons"></span> \(Sort\) to sort alphabetically.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    Filter


    
    </td>
    <td valign="top">

    In the *Filters* section, use one of the following filters:

    -   *Features* that a connection type supports \(*Remote Tables*, *Data Flows*, *Replication Flows*, *Model Import*\)

        For more information about the available features with SAP Datasphere, see [Supported Connection Type Features](integrating-data-via-connections-eb85e15.md#loioeb85e157ab654152bd68a8714036e463__section_connection_features).

    -   *Categories* that the corresponding source belongs to \(*On-Premise*, *Cloud*\)

    -   *Sources* that you would like to connect \(*SAP*, *Non-SAP*, *Partner Tools*\)



    
    </td>
    </tr>
    </table>
    
    > ### Note:  
    > When hovering over a connection type, an *Information* button appears that you can click to get information about the features supported by the connection type. This includes information about whether the connected system can be used as source and/or target.
    > 
    > In the information, a warning icon indicates if a feature is not available, and clicking the icon tells you what to do in that case. Also, if a connection type is inactive, the information tells you what to do to be able to use it.

4.  Complete the properties in the following sections and click *Next Step*.


    <table>
    <tr>
    <th valign="top">

    Property Section


    
    </th>
    <th valign="top">

    Description


    
    </th>
    </tr>
    <tr>
    <td valign="top">

    *Connection Details*


    
    </td>
    <td valign="top">

    Enter or select properties that are needed to locate the source system or database.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    Various


    
    </td>
    <td valign="top">

    Enter or select properties in additional sections depending on the connection type.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    *Credentials*


    
    </td>
    <td valign="top">

    Enter the credentials that are required to access the source.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    *Features*


    
    </td>
    <td valign="top">

    Select additional connection properties to enabe a feature, if required.

    You can click the info button next to the *Enabled* or *Disabled* information to get more information about what is required to enable the feature.


    
    </td>
    </tr>
    </table>
    
    > ### Note:  
    > If you connect to a partner tool, you will be redirected to an embedded partner UI to there enter credentials and required connection properties, if applicable.

    For an overview of all connection types including links to detailed property documentation, see [Connection Types Overview](integrating-data-via-connections-eb85e15.md#loioeb85e157ab654152bd68a8714036e463__section_connection_overview).

5.  \[optional\] For some connection types that use a Data Provisioning Agent to connect to the source, for example SAP ABAP, SAP HANA, or Microsoft SQL Server, you can define advanced properties which give you more control over your connectivity setup. If required, override default values according to your customer scenario’s needs, and then click *Next Step*.

6.  Complete the following properties:


    <table>
    <tr>
    <th valign="top">

    Property


    
    </th>
    <th valign="top">

    Description


    
    </th>
    </tr>
    <tr>
    <td valign="top">

    *Business Name*


    
    </td>
    <td valign="top">

    Enter a descriptive name to help users identify the object. This name can be changed at any time.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    *Technical Name*


    
    </td>
    <td valign="top">

    Displays the name used in scripts and code, synchronized by default with the *Business Name*.

    The technical name can only contain alphanumeric characters and underscores \(\_\). Underscore \(\_\) must not be used at the start or end of the name. The maximum length is 40 characters. The name must be unique within the space.

    > ### Note:  
    > Once the object is saved, the technical name can no longer be modified.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    *Description*


    
    </td>
    <td valign="top">

    Provide more information to help users understand the object.


    
    </td>
    </tr>
    </table>
    
7.  If you connect to a partner tool such as Precog, in the *Additional Configuration* section of this wizard step, you'll find information about IP addresses that you can copy in order to add them to the IP allowlist in SAP Datasphere.

    For more information, see [Add IP address to IP Allowlist](https://help.sap.com/viewer/935116dd7c324355803d4b85809cec97/internal/en-US/a3c214514ef94e899459f68f4c1e2a23.html "Clients in your local network need an entry in the appropriate IP allowlist in SAP Datasphere. Cloud Connectors in your local network only require an entry if you want to use them for federation and replication from on-premise systems.") :arrow_upper_right:.

8.  Click *Create Connection* to create the connection and add it to the overview of available connections.

    > ### Note:  
    > When creating a connection to a partner tool such as Precog, the system checks whether the required IP address or addresses are already available in the IP allowlist. Note that connection creation takes longer because checking the allowlist in the database requires some time.

9.  Select the connection and click <span class="SAP-icons"></span> \(Validate Connection\) to check if your connection is valid and can be used for the enabled features.

    > ### Note:  
    > When creating a connection to SAP HANA on-premise using SAP HANA smart data access via Cloud Connector, the system checks for a required internal service. In the connection overview, a warning icon indicates that the service might not be ready yet. This happens for the first connection you create or when you create a connection after the service has been disabled \(after an automated weekly check returning that there is no such connection anymore\). Getting the service ready might take up to 45 minutes. Validate the connection and check the message details for more information.




<a name="loioc2165842082c43fc85bad9f0c97572bb__result_ixt_zpk_r3b"/>

## Results

Depending on the connection type and the features that you have enabled for your connection:

-   You can use the connection either to import tables when creating views or ER models, to create data flows, or to create replication flows, or all three.

    For more information, see:

    -   [Importing Tables and Views from Sources](https://help.sap.com/viewer/24f836070a704022a40c15442163e5cf/internal/en-US/7c4acd33e39a451e99c87f0661772443.html "Import tables and views from a connection, Open SQL schema, HDI container or other source available in your space.") :arrow_upper_right:
    -   [Creating a Data Flow](https://help.sap.com/viewer/24f836070a704022a40c15442163e5cf/internal/en-US/e30fd1417e954577baae3246ea470c3f.html "Create a data flow to move and transform data in an intuitive graphical interface. You can drag and drop sources from the Source Browser, join them as appropriate, add other operators to remove or create columns, aggregate data, and do Python scripting, before writing the data to the target table.") :arrow_upper_right:
    -   [Creating a Replication Flow](https://help.sap.com/viewer/24f836070a704022a40c15442163e5cf/internal/en-US/25e2bd7a70d44ac5b05e844f9e913471.html "Create a replication flow if you want to copy data from a source to a target in a fast and easy way and do not require complex projections.") :arrow_upper_right:

    > ### Note:  
    > Generally, when importing a table, it is created as remote table. However, tables imported from partner tool connections are created as local tables \(see [Connections to Partner Tools](connections-to-partner-tools-55da0fa.md)\).

-   You can use remote tables imported from the connection either to access data directly live in the connected source \(federation\) or to copy the data into SAP Datasphere \(replication\).

    For more information, see [Replicating Data and Monitoring Remote Tables](../Data-Integration-Monitor/replicating-data-and-monitoring-remote-tables-4dd95d7.md).

-   You can use the connection to import entities from your source.

    For more information, see:

    -   [SAP BW∕4HANA Model Transfer](sap-bw-4hana-model-transfer-1caba95.md)
    -   [Importing SAP BW∕4HANA Models](https://help.sap.com/viewer/24f836070a704022a40c15442163e5cf/internal/en-US/a3d4a2f91bea4810ba8839ff73577dac.html "You can import existing analytic queries from SAP BW∕4HANA into SAP Datasphere in order to build new models on top of them or enhance them.") :arrow_upper_right:


