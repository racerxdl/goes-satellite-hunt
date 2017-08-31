# LRIT Header Description

As described in [File Header Processing](/file-assembler/file-header-processing.md), the LRIT File Header actually contains several header types with different sizes. All headers has _at least_ three starting bytes that represent the type and size of header:

| Field | Type | Description |
| :--- | :--- | :--- |
| Type | uint8\_t | Type of header \(see table below\) |
| Size | uint16\_t | Size of the entire header \(include these fields\) |
| Data | ? \(depends on type\) | Data of the header \(depends on type\) |

### Table 1 - Basic LRIT Header Structure

All the descriptions of headers will not include these two fields \(type and size\) since its common to **all** headers. The headers can be divided into two groups:

* [Primary Header](/file-types/lrit-header-description/primary-header.md)
* Secondary Headers

| Type | Name |
| :--- | :--- |
| 1 | [Image Structured Header](/file-types/lrit-header-description/1-image-structure-header.md) |
| 2 | [Image Navigation Record](/file-types/lrit-header-description/2-image-navigation-record.md) |
| 3 | [Image Data Function Record](/file-types/lrit-header-description/3-image-data-function-record.md) |
| 4 | [Annotation Record](/file-types/lrit-header-description/4-annotation-record.md) |
| 5 | [Timestamp Record](/file-types/lrit-header-description/5-timestamp-record.md) |
| 6 | [Ancillary Text](/file-types/lrit-header-description/6-ancillary-text.md) |
| 7 | [Key Header](/file-types/lrit-header-description/7-key-header.md) |
| 128 | [Segment Identification Header](/file-types/lrit-header-description/128-segment-identification-header.md) |
| 129 | [NOAA Specific Header](/file-types/lrit-header-description/129-noaa-specific-header.md) |
| 130 | [Header Structured Record](/file-types/lrit-header-description/130-header-structured-record.md) |
| 131 | [Rice Compression Record](/file-types/lrit-header-description/131-rice-compression-record.md) |
| 132 | [DCS Filename Record](/file-types/lrit-header-description/132-dcs-filename-record.md) |

### Table 2 - Secondary Header Types



