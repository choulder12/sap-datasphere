<!-- loio806d7f0c45a14f1fb07db0a226b2b822 -->

<link rel="stylesheet" type="text/css" href="../css/sap-icons.css"/>

# Monitoring Remote Queries

In the *Remote Query Monitor*, you track the queries sent to your remote connected source systems for your space. You can monitor the communication between the federation layer of SAP HANA Cloud and the connected remote source systems, and analyze them.

SAP Datasphere is connected to remote systems via SAP HANA Cloud using data federation. SAP HANA Cloud already provides a corresponding monitoring view of actual SAP HANA runtime data, including statistics and status information related to the execution of Data Manipulation Language \(DML\) statements. The *Remote Query Monitor* retrieves this information, so that you can keep an eye on how the communication between SAP Datasphere and the connected remote source systems is running and better analyze possibilities for performance bottlenecks while running queries in SAP Datasphere.

*Remote Query Monitor* allows you to monitor the queries sent to your remote connected source systems for your space. This information is helpful when analyzing executions of story \(or on views or previews\), since it provides details of single read requests, like runtimes or result set size.

> ### Note:  
> *Data Flows* executions are not contained in this monitoring view as *Data Flows* don't use SAP HANA Federation.

> ### Example:  
> You build a story on top on a view. In this story, you create charts and set filters on those charts. Let’s say you remove one of those filters. A query is then triggered to the connected remote source system. A new entry appears in the *Remote Query Monitor* and you can see the last statement sent by the story.

The *Remote Query Monitor* only shows the last 100 statements. It provides you with the following information:


<table>
<tr>
<th valign="top">

Column



</th>
<th valign="top">

Description



</th>
</tr>
<tr>
<td valign="top">

Connection



</td>
<td valign="top">

Displays the name of the connection. 



</td>
</tr>
<tr>
<td valign="top">

Start Time



</td>
<td valign="top">

Displays the statement start time. 



</td>
</tr>
<tr>
<td valign="top">

End Time



</td>
<td valign="top">

Displays the statement end time. 



</td>
</tr>
<tr>
<td valign="top">

Statement Runtime



</td>
<td valign="top">

Displays the duration of the statement. 



</td>
</tr>
<tr>
<td valign="top">

Rows



</td>
<td valign="top">

Displays the number of rows that have been processed by the statement. 



</td>
</tr>
<tr>
<td valign="top">

Status



</td>
<td valign="top">

Displays the status of the statement. 

The status can be one of the following:

-   *Closed*: The statement has been completed without error.
-   *Executing*: The statement is currently running.
-   *Error*: The statement can't be completed.



</td>
</tr>
<tr>
<td valign="top">

Remote SQL Statement



</td>
<td valign="top">

Displays the outgoing statement that is sent to the remote connected source system. 

As the statement is most often too long and appears as truncated, you need to click on *More* to get the full statement information.



</td>
</tr>
<tr>
<td valign="top">

Statement ID



</td>
<td valign="top">

Displays the ID of the statement. 

This ID is provided by SAP HANA and can be used to do deep dive analysis in the SAP HANA Cockpit. For more information, see [SAP HANA Cockpit](https://help.sap.com/viewer/6b94445c94ae495c83a19646e7c3fd56/latest/en-US/da25cad976064dc0a24a1b0ee9b62525.html).



</td>
</tr>
<tr>
<td valign="top">

Executing SQL Statement



</td>
<td valign="top">

Displays the statement that is currently running in SAP HANA Cloud, and which includes a remote SQL statement. 

You might have a look at this statement if something goes wrong to identify the root cause. As the statement is most often too long and appears as truncated, you need to click on *More* to get the full statement information.



</td>
</tr>
<tr>
<td valign="top">

Transaction



</td>
<td valign="top">

Displays the remote source transaction. 



</td>
</tr>
</table>

> ### Note:  
> You can personalize the columns you want to display and the display order of those columns clicking on :gear:.

