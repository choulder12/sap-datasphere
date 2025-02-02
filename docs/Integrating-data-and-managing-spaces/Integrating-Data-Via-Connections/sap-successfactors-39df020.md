<!-- loio39df02030d4b411487bacecf9afea4e8 -->

# SAP SuccessFactors

Use the connection to access employee-related data in SAP SuccessFactors.



<a name="loio39df02030d4b411487bacecf9afea4e8__section_um5_5lg_hsb"/>

## Prerequisites

See: [Prepare Connectivity to SAP SuccessFactors](https://help.sap.com/viewer/935116dd7c324355803d4b85809cec97/internal/en-US/c9b19156c417409b8d563cc4b56c5dc0.html "To be able to successfully validate and use a connection to SAP SuccessFactors for remote tables or data flows certain preparations have to be made.") :arrow_upper_right:



<a name="loio39df02030d4b411487bacecf9afea4e8__section_n34_dcc_x4b"/>

## Using the Connection

The connection type supports the remote table as well as the data flow feature.

Supported data access methods for remote tables:

-   Remote
-   Replication \(snapshot\)

    > ### Note:  
    > When replicating employee-related data, independently of their validity not only current data is replicated but all data including historical data.


For more information, see [Replicating Data and Monitoring Remote Tables](../Data-Integration-Monitor/replicating-data-and-monitoring-remote-tables-4dd95d7.md). 



<a name="loio39df02030d4b411487bacecf9afea4e8__section_irc_b54_npb"/>

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

 Enter the OData service provider URL of the SAP SuccessFactors service that you want to access. 

The syntax for the URL is: ****<SAP SuccessFactors API Server\>*/odata/v2/*<supported SAP SuccessFactors service group\>**** or ****<SAP SuccessFactors API Server\>*/odatav4/*<supported SAP SuccessFactors service group\>**** 



</td>
</tr>
<tr>
<td valign="top">

 *Version*  



</td>
<td valign="top">

 Displays the OData version used to implement the SAP SuccessFactors OData service. 



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

-   *User Name And Password* for basic authentication
-   *OAuth 2.0* 

The default is *OAuth 2.0*.

> ### Note:  
> HTTP basic authentication in SAP SuccessFactors will soon be retired. For more information, see [Deprecation of HTTP Basic Authentication](https://help.sap.com/doc/62fddbd651204629b46bbccbabf886ba/cloud/en-US/fcc05a902b4140e585d968c2fe4a96bc.html) in *SAP SuccessFactors What's New Viewer*.



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

Displays *SAML Bearer* as the grant type used to retrieve an access token. 



</td>
</tr>
<tr>
<td valign="top">

*OAuth Token Endpoint*



</td>
<td valign="top">

Enter the API endpoint to use to request an access token: ****<SAP SuccessFactors API Server\>*/oauth/token***.



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
<tr>
<td valign="top">

*OAuth API Endpoint*



</td>
<td valign="top">

> ### Caution:  
> Do not use the /oauth/idp API to generate SAML assertions. This approach is unsecure and has been deprecated.
> 
> For more information, see [Generating a SAML Assertion](https://help.sap.com/docs/SAP_SUCCESSFACTORS_PLATFORM/d599f15995d348a1b45ba5603e2aba9b/4e27e8f6ae2748ab9f23228dd6a31b06.html) in the *SAP SuccessFactors Platform* documentation.



</td>
</tr>
<tr>
<td valign="top">

*OAuth User ID*



</td>
<td valign="top">

Enter the SAP SuccessFactors user ID to use to request a SAML assertion.



</td>
</tr>
<tr>
<td valign="top">

*OAuth Company ID*



</td>
<td valign="top">

Enter the SAP SuccessFactors company ID \(identifying the SAP SuccessFactors system on the SAP SuccessFactors API server\) to use to request an access token.



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

Enter the API key received when registering SAP Datasphere as OAuth2 client application in SAP SuccessFactors. 



</td>
</tr>
<tr>
<td valign="top">

*Client Secret*



</td>
<td valign="top">

Enter the private key associated with the X.509 certificate for the registered OAuth2 client.



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

 Enter the user name in *<username@companyID\>* format. 



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

*Data Flows* are enabled without the need to set any additional connection properties.

