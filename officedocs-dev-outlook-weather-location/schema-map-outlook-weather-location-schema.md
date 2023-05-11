﻿---
title: Schema map (Outlook Weather Location Schema)
TOCTitle: Schema map
ms:assetid: 1a5195ae-7905-477a-7818-9eb3bff64af0
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ227768(v=office.15)
ms:contentKeyID: 48463652
ms.date: 07/24/2014
mtps_version: v=office.15
dev_langs:
- xml
---

# Schema map (Outlook Weather Location Schema)

This topic shows the schema definition for the Outlook Weather Location XML Schema.

``` xml
<?xml version="1.0" ?>
<xs:schema
  attributeFormDefault="unqualified" elementFormDefault="qualified"
xmlns:xs="http://www.w3.org/2001/XMLSchema"
targetNamespace= "http://schemas.microsoft.com/office/outlook/15/getweatherlocation.xsd"
xmlns="http://schemas.microsoft.com/office/outlook/15/getweatherlocation.xsd"
>
  <!-- get weather location  -->
  <!-- example query: http://weather.service.msn.com/data.aspx?outputview=search&weasearchstr=tsurumi -->
  
  <xs:element name="weatherdata">
    <xs:annotation>
      <xs:documentation>Defines the weather element.</xs:documentation>
    </xs:annotation>
    <xs:complexType>
      <xs:sequence>
        <xs:element name="weather" type="weatherType" maxOccurs="unbounded">
          <xs:annotation>
            <xs:documentation>Specifies the location to report weather on.</xs:documentation>
          </xs:annotation>
        </xs:element>
      </xs:sequence>
    </xs:complexType>
  </xs:element>

  <xs:complexType name="weatherType">
    <xs:annotation>
      <xs:documentation> Defines the parameters about the weather conditions of a location.</xs:documentation>
    </xs:annotation>

    <xs:attribute name="weatherlocationname" type="xs:string" use="required">
      <xs:annotation>
        <xs:documentation>Specifies the name of the location.</xs:documentation>
      </xs:annotation>
    </xs:attribute>
    <xs:attribute name="weatherlocationcode" type="xs:string" use="required">
      <xs:annotation>
        <xs:documentation>Specifies a code that is associated with the location to distinguish multiple locations with the same name. </xs:documentation>
      </xs:annotation>
    </xs:attribute>
  </xs:complexType>
</xs:schema>
```

