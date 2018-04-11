---
title: weather element (weatherdata element) (Outlook Weather Location Schema)
TOCTitle: weather element
ms:assetid: 1127956a-37aa-c39e-60b4-343dcc4ead82
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ227504(v=office.15)
ms:contentKeyID: 48461610
ms.topic: Archived
ms.date: 07/24/2014
mtps_version: v=office.15
dev_langs:
- xml
---

# weather element (weatherdata element) (Outlook Weather Location Schema)

Specifies the location to report weather on.

## Element information

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Element type</strong></p></td>
<td><p><a href="weathertype-complextype-outlook-weather-location-schema.md">weatherType</a></p></td>
</tr>
<tr class="even">
<td><p><strong>Namespace</strong></p></td>
<td><p>http://schemas.microsoft.com/office/outlook/15/getweatherlocation.xsd</p></td>
</tr>
<tr class="odd">
<td><p><strong>Schema file</strong></p></td>
<td><p>getweatherlocation.xsd</p></td>
</tr>
</tbody>
</table>

## Definition

``` xml
<xs:element name="weather"      type="weatherType" maxOccurs="unbounded"    >


  </xs:element>  
```

## Elements and attributes

If the schema defines specific requirements, such as sequence, minOccurs, maxOccurs, and choice, see the definition section.

### Parent elements

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Element</p></th>
<th><p>Type</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="weatherdata-element-outlook-weather-location-schema.md">weatherdata</a></p></td>
<td></td>
<td><p>Defines the weather element.</p></td>
</tr>
</tbody>
</table>

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

