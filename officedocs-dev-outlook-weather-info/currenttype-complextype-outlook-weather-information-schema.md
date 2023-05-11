---
title: currentType complexType (Outlook Weather Information Schema)
TOCTitle: currentType complexType
ms:assetid: 9f4663ac-13d3-6c46-f839-ba6bca4047a3
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ230328(v=office.15)
ms:contentKeyID: 48483105
ms.date: 07/24/2014
mtps_version: v=office.15
dev_langs:
- xml
---

# currentType complexType (Outlook Weather Information Schema)

Defines the parameters about the current weather conditions of a location.

## Type information

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Namespace</strong></p></td>
<td><p>http://schemas.microsoft.com/office/outlook/15/getweatherinfo.xsd</p></td>
</tr>
<tr class="even">
<td><p><strong>Schema file</strong></p></td>
<td><p>getweatherinfo.xsd</p></td>
</tr>
<tr class="odd">
<td><p><strong>Extension base</strong></p></td>
<td><p>None</p></td>
</tr>
</tbody>
</table>

## Definition

``` xml

       <xs:complexType name="currentType">
     <xs:attribute name="winddisplay"   type="xs:string"      use="required"     />
     <xs:attribute name="windspeed"   type="xs:integer"      use="required"     />
     <xs:attribute name="humidity"   type="xs:integer"      use="required"     />
     <xs:attribute name="feelslike"   type="xs:integer"      use="required"     />
     <xs:attribute name="observationpoint"   type="xs:string"      use="required"     />
     <xs:attribute name="observationtime"   type="xs:time"      use="required"     />
     <xs:attribute name="date"   type="xs:date"      use="required"     />
     <xs:attribute name="skytext"   type="xs:string"      use="required"     />
     <xs:attribute name="skycode"   type="xs:integer"      use="required"     />
     <xs:attribute name="temperature"   type="xs:integer"      use="required"     />
     <xs:attribute name="shortday"   type="xs:string"      use="optional"     />
     <xs:attribute name="day"   type="xs:string"      use="optional"     />
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
<td><p>date</p></td>
<td><p>xs:date</p></td>
<td><p>required</p></td>
<td><p>Specifies today's date.</p></td>
<td><p>A value of the type xs:date</p></td>
</tr>
<tr class="even">
<td><p>day</p></td>
<td><p>xs:string</p></td>
<td><p>optional</p></td>
<td><p>Specifies a day for the forecast.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
<tr class="odd">
<td><p>feelslike</p></td>
<td><p>xs:integer</p></td>
<td><p>required</p></td>
<td><p>Specifies the temperature of how the current weather feels like.</p></td>
<td><p>A value of the type xs:integer</p></td>
</tr>
<tr class="even">
<td><p>humidity</p></td>
<td><p>xs:integer</p></td>
<td><p>required</p></td>
<td><p>Specifies the current numerical humidity value.</p></td>
<td><p>A value of the type xs:integer</p></td>
</tr>
<tr class="odd">
<td><p>observationpoint</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>Specifies where the current weather information is observed from.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
<tr class="even">
<td><p>observationtime</p></td>
<td><p>xs:time</p></td>
<td><p>required</p></td>
<td><p>Specifies when the current weather information is observed at.</p></td>
<td><p>A value of the type xs:time</p></td>
</tr>
<tr class="odd">
<td><p>shortday</p></td>
<td><p>xs:string</p></td>
<td><p>optional</p></td>
<td><p>Specifies a day in abbreviated form.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
<tr class="even">
<td><p>skycode</p></td>
<td><p>xs:integer</p></td>
<td><p>required</p></td>
<td><p>Specifies an integer code for the current weather conditions.</p></td>
<td><p>A value of the type xs:integer</p></td>
</tr>
<tr class="odd">
<td><p>skytext</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>Specifies one to two words describing current weather conditions.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
<tr class="even">
<td><p>temperature</p></td>
<td><p>xs:integer</p></td>
<td><p>required</p></td>
<td><p>Specifies the current temperature of the location.</p></td>
<td><p>A value of the type xs:integer</p></td>
</tr>
<tr class="odd">
<td><p>winddisplay</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>A string that describes the current wind conditions.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
<tr class="even">
<td><p>windspeed</p></td>
<td><p>xs:integer</p></td>
<td><p>required</p></td>
<td><p>Specifies the current numerical wind speed value.</p></td>
<td><p>A value of the type xs:integer</p></td>
</tr>
</tbody>
</table>

