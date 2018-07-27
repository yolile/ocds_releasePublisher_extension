## Release Publishers Extension
### Description
Includes the information about the publisher at release level for the cases in that a release-package or record-packages 
contains releases from different publishers.

In a compileRelease could be more than one publisher, for that, the publishers field is an array

### Fields
- release.publishers: Information to uniquely identify the publisher(s) of this release.

### Example

```javascript
{
    "publisher": {
        "name": "SECRETARÍA DE LA FUNCIÓNN PÚBLICA / SECRETARIA DE HACIENDA Y CRÉDITO PÚBLICO", 
        "uri": "http://www.gob.mx/contratacionesabiertas/"
    }, 
    "license": "https://datos.gob.mx/libreusomx", 
    "publishedDate": "2018-02-14T19:23:19.405517Z", 
    "uri": "https://api.datos.gob.mx/v1/", 
    "records": [
        {
            "ocid": "ocds-07smqs-1303516", 
            "releases": [
                {
                    "publishers": [{
                        "id" : 1,
                        "uri": "http://www.gob.mx/sfp", 
                        "uid": "27511", 
                        "name": "SECRETARÍA DE LA FUNCIÓN PÚBLICA"
                        }], 
                    "language": "es"
                    ....
                }, 
                {
                    "publishers": [{
                        "id": 1
                        "uri": "http://www.gob.mx/shcp", 
                        "uid": "00000", 
                        "name": "SECRETARÍA DE HACIENDA Y CRÉDITO PÚBLICO"
                        }], 
                    "language": "es"
                    ....
                }
            ]
        }
    ]
}
```