# Primary Header

The Primary Header group is a _single_ header that contains:

* **Header Type** - Always 0
* **File Type Code** - Type Code of the file content
* **Header Length** - Combined Size of Primary + Secondary Headers
* **Data Length** - Size of the data inside this file

The File Type Code is a ENUM that contains the following values:

| Name | Value |
| :--- | :--- |
| Image | 0 |
| Messages | 1 |
| Text | 2 |
| Encryption Key | 3 |
| Reserved | 4 |
| Meteorological Data | 128 |
| DCS | 130 |
| EMWIN | 214 |

###### Table 1 - FileTypeCode ENUM Values

---

Sadly, at least NOAA Stations for GOES 13 / 16 doesn't always follow that file type codes, so I usually ignore them or just use for a preliminary processing just for display purpose. For example a EMWIN data might come with a Meteorological Data. There is other ways to detect the file type that will be described later, so I do not recommend using this field for checking the content type.

