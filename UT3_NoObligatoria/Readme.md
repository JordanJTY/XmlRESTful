# Las Palmas de Gran Canaria Local Police attestations 2014

### Description

These xml are used to save the data of Police attestations on 2014 in Las Palmas de Gran Canaria.

### Screenshots

* XML:

![create product](https://github.com/tcrurav/XmlRESTfulNodeJSfromJS/blob/master/web/img/create_product.png)

* XSD:

![show products](https://github.com/tcrurav/XmlRESTfulNodeJSfromJS/blob/master/web/img/show_products.png)

### XML and XSD files 
XML:

```
<?xml version="1.0" encoding="UTF-8"?>
<atestado>
        <DILIG>5</DILIG>
        <LUGAR>PUENTE ELEVADO LA BALLENA</LUGAR>
        <ALTURA_DE />
        <FECHA>2014-01-01T00:00:00</FECHA>
        <HORA>06:20</HORA>
        <VEHICULOS>2</VEHICULOS>
        <HERIDOS>1</HERIDOS>
        <DESTINO>Jefatura</DESTINO>
        <COLISION>Colisión</COLISION>
        <INFR_COND>No mantener el intervalo seg.</INFR_COND>
        <INFR_PEAT>Ninguna infracción</INFR_PEAT>
        <DENUNCIAS>0</DENUNCIAS>
    </atestado>
```

XSD:

```
<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" targetNamespace="https://www.jordancio.com"
    xmlns="https://www.jordancio.com" elementFormDefault="qualified">
    <xs:element name="atestados">
        <xs:complexType>
            <xs:sequence>
                <xs:element name="atestado" minOccurs="1" maxOccurs="unbounded">
                    <xs:complexType>
                        <xs:sequence>
                            <xs:element name="DILIG"></xs:element>
                            <xs:element name="LUGAR"></xs:element>
                            <xs:element name="ALTURA_DE"></xs:element>
                            <xs:element name="FECHA"></xs:element>
                            <xs:element name="HORA"></xs:element>
                            <xs:element name="VEHICULOS"></xs:element>
                            <xs:element name="HERIDOS"></xs:element>
                            <xs:element name="DESTINO"></xs:element>
                            <xs:element name="COLISION"></xs:element>
                            <xs:element name="INFR_COND"></xs:element>
                            <xs:element name="INFR_PEAT"></xs:element>
                            <xs:element name="DENUNCIAS"></xs:element>
                        </xs:sequence>
                    </xs:complexType>
                </xs:element>
            </xs:sequence>
        </xs:complexType>
    </xs:element>
</xs:schema>
```

# Validation screenshots

A validation of xml. 

![validation test](https://github.com/tcrurav/XmlRESTfulNodeJSfromJS/blob/master/web/img/products_validation.png)

## Acknowledgments

* http://datosabiertos.laspalmasgc.es/resource/?ds=atestados-policia-local-2014&id=999fbede-ec95-4493-9e5b-4d9806a5e103&ft=XML. Where I find all info.
* https://github.com/tcrurav/XmlRESTfulNodeJSfromJS. Example I used to do this project.
* https://www.w3schools.com/xml/default.asp. Info about how to use XML.
* https://www.w3schools.com/xml/schema_intro.asp. Info about how to use XSD.
* https://opendata.esri.es. Another web where we can get more info about OpenData.
* I used Visual Studio Code to do this project.