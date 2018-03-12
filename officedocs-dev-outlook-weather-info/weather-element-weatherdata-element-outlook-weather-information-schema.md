---
title: weather element (weatherdata element) (Outlook Weather Information Schema)
TOCTitle: weather element
ms:assetid: de3c35ef-84a3-b991-7c98-3eca720c9ba0
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ231205(v=office.15)
ms:contentKeyID: 48489065
ms.date: 07/24/2014
mtps_version: v=office.15
dev_langs:
- xml
---

# weather element (weatherdata element) (Outlook Weather Information Schema)

Specifies the weather conditions of a location.

## Element information

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Element type</strong></p></td>
<td><p><a href="weathertype-complextype-outlook-weather-information-schema.md">weatherType</a></p></td>
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
<xs:element name="weather"      type="weatherType">


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
<td><p><a href="weatherdata-element-outlook-weather-information-schema.md">weatherdata</a></p></td>
<td></td>
<td><p>Defines the weather element.</p></td>
</tr>
</tbody>
</table>

### Child elements

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
<td><p><a href="current-element-weathertype-complextype-outlook-weather-information-schema.md">current</a></p></td>
<td><p><a href="currenttype-complextype-outlook-weather-information-schema.md">currentType</a></p></td>
<td><p>Specifies the current weather conditions.</p></td>
</tr>
<tr class="even">
<td><p><a href="forecast-element-weathertype-complextype-outlook-weather-information-schema.md">forecast</a></p></td>
<td><p><a href="forecasttype-complextype-outlook-weather-information-schema.md">forecastType</a></p></td>
<td><p>Specifies the future weather conditions of at least three days ahead including today: Today, Tomorrow, Day after Tomorrow.</p></td>
</tr>
</tbody>
</table>

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
<td><p>attribution</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>Specifies the source of the weather information.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
<tr class="even">
<td><p>degreetype</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>Specifies the unit for the temperature of the location for example, Celsius.</p></td>
<td><p>C, F</p></td>
</tr>
<tr class="odd">
<td><p>imagerelativeurl</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>Specifies the URL of the image for the location.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
<tr class="even">
<td><p>timezone</p></td>
<td><p>xs:integer</p></td>
<td><p>required</p></td>
<td><p>Specifies the GMT offset.</p></td>
<td><p>A value between -11 and 12 inclusive</p></td>
</tr>
<tr class="odd">
<td><p>url</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>Specifies the URL for the web page of the weather service that contains weather information for the specified location.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
<tr class="even">
<td><p>weatherlocationcode</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>Specifies the code that is associated with the location used to distinguish multiple location that have the same name.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
<tr class="odd">
<td><p>weatherlocationname</p></td>
<td><p>xs:string</p></td>
<td><p>required</p></td>
<td><p>Specifies the name of the location that appears in the drop-down control.</p></td>
<td><p>A value of the type xs:string</p></td>
</tr>
</tbody>
</table>

