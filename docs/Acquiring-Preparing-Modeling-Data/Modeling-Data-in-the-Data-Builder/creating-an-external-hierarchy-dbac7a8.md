<!-- loiodbac7a862b3744d8a71d268644aac389 -->

<link rel="stylesheet" type="text/css" href="../css/sap-icons.css"/>

# Creating an External Hierarchy

Select a *Semantic Usage* of *Hierarchy* to indicate that your entity contains parent-child relationships for members in a dimension.



## Procedure

1.  Open the table or view containing the hierarchy information and set the following properties:


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

    Business Name


    
    </td>
    <td valign="top">

    Enter a descriptive name to help users identify the object. This name can be changed at any time.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    Technical Name


    
    </td>
    <td valign="top">

    Displays the name used in scripts and code, synchronized by default with the *Business Name*.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    Semantic Usage


    
    </td>
    <td valign="top">

    Choose *Hierarchy*.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    Parent Column / Child Column


    
    </td>
    <td valign="top">

    Select the columns containing the parent and child information for your hierarchy.

    > ### Note:  
    > The parent column and the child column must be of the same data type.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    Expose for Consumption


    
    </td>
    <td valign="top">

    In order to consume your hierarchy in SAP Analytics Cloud, you must enable the *Expose for Consumption* switch.


    
    </td>
    </tr>
    </table>
    
2.  Set attributes as keys to indicate that the data they contain can uniquely identify records.

    > ### Note:  
    > You must set exactly one key attribute for a *Hierarchy*:
    > 
    > -   Child attribute of the parent-child hierarchy structure

    To set an attribute as a key column, select the checkbox in the *Key* column or hover over the attribute in the side panel and click <span class="FPA-icons"></span> \(Menu\)** \> *Set as Key*.

3.  Click <span class="FPA-icons"></span> \(Save\) to save your entity:

    -   *Save* to save your object.
    -   *Save As* to create a local a copy of the object you're working on. The object must have been previously saved at least once. The *Save* dialog opens. Enter new business and technical names and click *Save*.

    Click <span class="SAP-icons"></span> \(Deploy\) to deploy your entity.


