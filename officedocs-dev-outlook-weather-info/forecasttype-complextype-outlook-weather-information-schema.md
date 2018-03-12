---
title: forecastType complexType (Outlook Weather Information Schema)
TOCTitle: forecastType complexType
ms:assetid: 6301d6b6-34fa-af8d-e682-605d35cfdf47
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ229138(v=office.15)
ms:contentKeyID: 48474083
ms.date: 07/24/2014
mtps_version: v=office.15
dev_langs:
- xml
---

# forecastType complexType (Outlook Weather Information Schema)

Defines the parameters about the forecast weather conditions of a location.

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

       <xs:complexType name="forecastType">
     <xs:attribute name="shortday"   type="xs:string"      use="required"     />
     <xs:attribute name="day"   type="xs:string"      use="required"     />
     <xs:attribute name="date"   type="xs:date"      use="required"     />
     <xs:attribute name="precip"   type="xs:integer"      use="required"     />
     <xs:attribute name="skytextday"   type="xs:string"      use="required"     />
     <xs:attribute name="skycodeday"   type="xs:integer"      use="required"     />
     <xs:attribute name="high"   type="xs:integer"      use="required"     />
     <xs:attribute name="low"   type="xs:integer"      use="required"     />
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
<td><p>Specifies the date for the forecast.</p></td>
<td><p>A value of the type xs:date</p></td>
</tr>
<tr class="even">
<td><p>day</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>Specifies a day for the forecast.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
<tr class="odd">
<td><p>high</p></td>
<td><p>xs:integer</p></td>
<td><p>required</p></td>
<td><p>Specifies the forecasted highest temperature.</p></td>
<td><p>A value of the type xs:integer</p></td>
</tr>
<tr class="even">
<td><p>low</p></td>
<td><p>xs:integer</p></td>
<td><p>required</p></td>
<td><p>Specifies the forecasted lowest temperature.</p></td>
<td><p>A value of the type xs:integer</p></td>
</tr>
<tr class="odd">
<td><p>precip</p></td>
<td><p>xs:integer</p></td>
<td><p>required</p></td>
<td><p>Specifies the percentage possibility of precipitation.</p></td>
<td><p>A value of the type xs:integer</p></td>
</tr>
<tr class="even">
<td><p>shortday</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>Specifies a day in abbreviated form.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
<tr class="odd">
<td><p>skycodeday</p></td>
<td><p>xs:integer</p></td>
<td><p>required</p></td>
<td><p>Specifies a code for the forecasted conditions.</p></td>
<td><p>A value of the type xs:integer</p></td>
</tr>
<tr class="even">
<td><p>skytextday</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>Specifies one to two words that describe the forecasted conditions.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
</tbody>
</table>

