<!-- loio5d36f1aae68a4e59989c424a66d948c9 -->

# Generic OData

Use the connection to access data from an OData service. 



<a name="loio5d36f1aae68a4e59989c424a66d948c9__section_j1b_byq_spb"/>

## Prerequisites

See: [Prepare Connectivity for Generic OData](https://help.sap.com/viewer/935116dd7c324355803d4b85809cec97/internal/en-US/d9c43a2dd2b340c48e4e665967c853e8.html "To be able to successfully validate and use a connection to an OData service for remote tables or data flows certain preparations have to be made.") :arrow_upper_right:



<a name="loio5d36f1aae68a4e59989c424a66d948c9__Odata_usage"/>

## Using the Connection

The connection type supports the remote table as well as the data flow feature.

Supported data access methods for remote tables:

-   Remote
-   Replication \(snapshot\)

For more information, see [Replicating Data and Monitoring Remote Tables](../Data-Integration-Monitor/replicating-data-and-monitoring-remote-tables-4dd95d7.md). 



<a name="loio5d36f1aae68a4e59989c424a66d948c9__section_nrb_hcc_x4b"/>

## Configuring Connection Properties



### Connection Details


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

 *URL*  



</td>
<td valign="top">

 Enter the OData service provider URL. 

> ### Note:  
> The OData service URL needs to be publicly available.



</td>
</tr>
<tr>
<td valign="top">

 *Version*  



</td>
<td valign="top">

 Select the OData version used to implement the OData service \(*V2* or *V4*\). 



</td>
</tr>
</table>



### Cloud Connector


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

 *Use Cloud Connector* 



</td>
<td valign="top">

 Set to *true* if your source is an on-premise source and you want to use the connection for data flows. The default is *false*. 



</td>
</tr>
<tr>
<td valign="top">

 \[if *Use Cloud Connector* = *true*\] *Location* 



</td>
<td valign="top">

 Select a location. 



</td>
</tr>
<tr>
<td valign="top">

 \[if *Use Cloud Connector* = *true*\] *Virtual Destination* 



</td>
<td valign="top">

 Select *Derive Virtual Host and Port from Connection Details* or *Enter Virtual Host and Port in Separate Fields*. 

If host and port entered in the connection details match the virtual host and port from the Cloud Connector configuration, you can select *Derive Virtual Host and Port from Connection Details* and don't need to enter the values manually.



</td>
</tr>
<tr>
<td valign="top">

 \[if *Virtual Destination* = *Enter Virtual Host and Port in Separate Fields*\] *Virtual Host* 



</td>
<td valign="top">

 Enter the virtual host that you defined during Cloud Connector configuration. 



</td>
</tr>
<tr>
<td valign="top">

 \[if *Virtual Destination* = *Enter Virtual Host and Port in Separate Fields*\] *Virtual Port* 



</td>
<td valign="top">

 Enter the virtual port that you defined during Cloud Connector configuration. 



</td>
</tr>
</table>



### Authentication


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

*Authentication Type*



</td>
<td valign="top">

Select the authentication type to use to connect to the OData endpoint. 

You can select:

-   *No Authentication*
-   *User Name And Password* for basic authentication
-   *OAuth 2.0* 

The default is *OAuth 2.0*.



</td>
</tr>
</table>



### OAuth 2.0

If *Authentication Type* = *OAuth 2.0*:


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

*OAuth Grant Type*



</td>
<td valign="top">

Displays *Client Credentials* as grant type used to retrieve an access token. 



</td>
</tr>
<tr>
<td valign="top">

*OAuth Token Endpoint*



</td>
<td valign="top">

Enter the API endpoint to use to request an access token.



</td>
</tr>
<tr>
<td valign="top">

*OAuth Scope*



</td>
<td valign="top">

\[optional\] Enter the OAuth scope, if applicable.



</td>
</tr>
</table>



### Credentials \(OAuth 2.0\)

If *Authentication Type* = *OAuth 2.0*:


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

*Client ID*



</td>
<td valign="top">

Enter the client ID to authenticate SAP Datasphere to the authorization server. 



</td>
</tr>
<tr>
<td valign="top">

*Client Secret*



</td>
<td valign="top">

Enter the client secret to authenticate SAP Datasphere to the authorziation server.



</td>
</tr>
</table>



### Credentials \(User Name And Password\)

If *Authentication Type* = *User Name And Password*:


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

 *User Name*  



</td>
<td valign="top">

 Enter the user name. 



</td>
</tr>
<tr>
<td valign="top">

 *Password*  



</td>
<td valign="top">

 Enter the password. 



</td>
</tr>
</table>



### Features

*Remote Tables* are enabled without the need to set any additional connection properties.

*Data Flows* are enabled without the need to set any additional connection properties. If your source is an on-premise source, make sure you have maintained the properties in the *Cloud Connector* section.

