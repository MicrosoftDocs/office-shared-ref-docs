---
title: weatherdata element (Outlook Weather Location Schema)
TOCTitle: weatherdata element
ms:assetid: 14e0c469-31dc-fbe2-0d45-da602df04f13
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ227596(v=office.15)
ms:contentKeyID: 48462300
ms.topic: Archived
ms.date: 07/24/2014
mtps_version: v=office.15
dev_langs:
- xml
---

# weatherdata element (Outlook Weather Location Schema)

Defines the weather element.

## Element information

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Element type</strong></p></td>
<td></td>
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
    <xs:element name="weatherdata"
    >
          <xs:complexType>
          <xs:sequence>
    <xs:element name="weather"
     type="weatherType" maxOccurs="unbounded"
      >
    </xs:element>
    
      </xs:sequence>
      </xs:complexType>
    </xs:element>
    
```

## Elements and attributes

If the schema defines specific requirements, such as sequence, minOccurs, maxOccurs, and choice, see the definition section.

### Parent elements

None.

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
<td><p><a href="weather-element-weatherdata-element-outlook-weather-location-schema.md">weather</a></p></td>
<td><p><a href="weathertype-complextype-outlook-weather-location-schema.md">weatherType</a></p></td>
<td><p>Specifies the location to report weather on.</p></td>
</tr>
</tbody>
</table>

### Attributes

None.

