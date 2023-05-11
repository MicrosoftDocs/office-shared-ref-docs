---
title: current element (weatherType complexType) (Outlook Weather Information Schema)
TOCTitle: current element
ms:assetid: d592a396-f935-c44c-409f-b849c327cfbd
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ231071(v=office.15)
ms:contentKeyID: 48488309
ms.date: 07/24/2014
mtps_version: v=office.15
dev_langs:
- xml
---

# current element (weatherType complexType) (Outlook Weather Information Schema)

Specifies the current weather conditions.

## Element information

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Element type</strong></p></td>
<td><p><a href="currenttype-complextype-outlook-weather-information-schema.md">currentType</a></p></td>
</tr>
<tr class="even">
<td><p><strong>Namespace</strong></p></td>
<td><p>http://schemas.microsoft.com/office/outlook/15/getweatherinfo.xsd</p></td>
</tr>
<tr class="odd">
<td><p><strong>Schema file</strong></p></td>
<td><p>getweatherinfo.xsd</p></td>
</tr>
</tbody>
</table>

## Definition

``` xml
<xs:element name="current"      type="currentType">


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
<td><p><a href="weather-element-weatherdata-element-outlook-weather-information-schema.md">weather</a></p></td>
<td><p><a href="weathertype-complextype-outlook-weather-information-schema.md">weatherType</a></p></td>
<td><p>Specifies the weather conditions of a location.</p></td>
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

