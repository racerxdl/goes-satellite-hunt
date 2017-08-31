# Annotation Record

The annotation record is used for defining a filename for the LRIT file. It is optional according to LRIT specification but all files received so far contains it. For DCS Files this should be overrided with [DCS FIlename Record](/file-types/lrit-header-description/132-dcs-filename-record.md), since DCS files will also contain this field, but after content is extracted it should be named as the DCS Filename Header says.

| Name | Type | Description |
| :--- | :--- | :--- |
| Filename | string \(64\) | The Filename |

### Table 9 - Annotation Record Fields



