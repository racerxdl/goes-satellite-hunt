# Timestamp Record

This timestamp record contains a packed timestamp in CCSDS Time format.

| Name | Type | Description |
| :--- | :--- | :--- |
| days | uint16\_t | Number of days since January 1st, 1958 |
| ms | uint32\_t | Number of milliseconds of the day |

### Table 10 - Timestamp Record Fields

This timestamp is sent using a UTC timezone \(GMT\) but it's not always present in all files.

