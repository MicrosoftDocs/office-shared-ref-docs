---
title: weatherType complexType (Outlook Weather Information Schema)
TOCTitle: weatherType complexType
ms:assetid: b94d848e-868a-5d5e-ad82-39ed9bd5b357
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ230745(v=office.15)
ms:contentKeyID: 48485978
ms.date: 07/24/2014
mtps_version: v=office.15
dev_langs:
- xml
---

# weatherType complexType (Outlook Weather Information Schema)

Specifies the weather conditions of a location.

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

           <xs:complexType name="weatherType">
           <xs:sequence>
     <xs:element name="current"      type="currentType">


  </xs:element>  
     <xs:element name="forecast"      type="forecastType" minOccurs="3"     maxOccurs="unbounded"    >


  </xs:element>  
       </xs:sequence>
     <xs:attribute name="weatherlocationcode"   type="xs:string"      use="required"     />
     <xs:attribute name="timezone"   type="xs:integer"      use="required"     />
     <xs:attribute name="attribution"   type="xs:string"      use="required"     />
     <xs:attribute name="degreetype"   type="xs:string"      use="required"     />
     <xs:attribute name="imagerelativeurl"   type="xs:string"      use="required"     />
     <xs:attribute name="url"   type="xs:string"      use="required"     />
     <xs:attribute name="weatherlocationname"   type="xs:string"      use="required"     />
       </xs:complexType>
```

## Elements and attributes

If the schema defines specific requirements, such as sequence, minOccurs, maxOccurs, and choice, see the definition section.

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

