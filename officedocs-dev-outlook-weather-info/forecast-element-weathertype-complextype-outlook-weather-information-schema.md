---
title: forecast element (weatherType complexType) (Outlook Weather Information Schema)
TOCTitle: forecast element
ms:assetid: 9124fa30-d58b-8354-91e9-8d2237a8251d
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ230033(v=office.15)
ms:contentKeyID: 48480955
ms.date: 07/24/2014
mtps_version: v=office.15
dev_langs:
- xml
---

# forecast element (weatherType complexType) (Outlook Weather Information Schema)

Specifies the future weather conditions of at least three days ahead including today: Today, Tomorrow, Day after Tomorrow.

## Element information

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Element type</strong></p></td>
<td><p><a href="forecasttype-complextype-outlook-weather-information-schema.md">forecastType</a></p></td>
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
<xs:element name="forecast"      type="forecastType" minOccurs="3"     maxOccurs="unbounded"    >


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

