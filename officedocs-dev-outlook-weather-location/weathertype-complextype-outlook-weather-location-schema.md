---
title: weatherType complexType (Outlook Weather Location Schema)
TOCTitle: weatherType complexType
ms:assetid: f8054fd9-85ba-fcf6-c96d-a54095d5238c
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ231497(v=office.15)
ms:contentKeyID: 48491372
ms.date: 07/24/2014
mtps_version: v=office.15
dev_langs:
- xml
---

# weatherType complexType (Outlook Weather Location Schema)

Defines the parameters about the weather conditions of a location.

## Type information

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Namespace</strong></p></td>
<td><p>http://schemas.microsoft.com/office/outlook/15/getweatherlocation.xsd</p></td>
</tr>
<tr class="even">
<td><p><strong>Schema file</strong></p></td>
<td><p>getweatherlocation.xsd</p></td>
</tr>
<tr class="odd">
<td><p><strong>Extension base</strong></p></td>
<td><p>None</p></td>
</tr>
</tbody>
</table>

## Definition

``` xml

       <xs:complexType name="weatherType">
     <xs:attribute name="weatherlocationname"   type="xs:string"      use="required"     />
     <xs:attribute name="weatherlocationcode"   type="xs:string"      use="required"     />
       </xs:complexType>
```

## Elements and attributes

If the schema defines specific requirements, such as sequence, minOccurs, maxOccurs, and choice, see the definition section.

### Child elements

None.

### Attributes

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Attribute</p></th>
<th><p>Type</p></th>
<th><p>Required</p></th>
<th><p>Description</p></th>
<th><p>Possible values</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>weatherlocationcode</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>Specifies a code that is associated with the location to distinguish multiple locations with the same name.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
<tr class="even">
<td><p>weatherlocationname</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>Specifies the name of the location.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
</tbody>
</table>

