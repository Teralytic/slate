---

title: teralytic-api

language_tabs:
   - shell
   - python
   - javascript

toc_footers:
   - <a href='#'>Sign Up for a Developer Key</a>
   - <a href='https://github.com/lavkumarv'>Documentation Powered by lav</a>

includes:
   - errors

search: true

---

# Introduction

Teralytic-API allows customers and partners to view their probes, the sensor readings, as well as analytics and calculations from Teralytic algorithms.

**Version:** 1.0

# /organizations
## ***GET***

**Summary:** List All Organizations associated with account key

### HTTP Request
`***GET*** /organizations`

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Successful Response |

# /organization/{id}
## ***GET***

**Summary:** List All Organizations associated with account key

### HTTP Request
`***GET*** /organization/{id}`

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path | id of organization to retrieve | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Successful Response |

# /fields
## ***GET***

**Summary:** List All Fields associated with account key

### HTTP Request
`***GET*** /fields`

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Successful Response |

## ***POST***

**Summary:** List All fields that intersect with polygon (array of lat/lng)

### HTTP Request
`***POST*** /fields`

**Responses**

| Code | Description |
| ---- | ----------- |
| 201 | Successful Response |

# /field/{id}
## ***GET***

**Summary:** List Field Details associated with id provided and within those associated with the account key

### HTTP Request
`***GET*** /field/{id}`

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path | id of field to retrieve | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Successful Response |

# /probes
## ***GET***

**Summary:** List All Probes associated with account key

### HTTP Request
`***GET*** /probes`

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Successful Response |

## ***POST***

**Summary:** List all probes associated with this key within a polygon (array of lat/lng)

### HTTP Request
`***POST*** /probes`

**Responses**

| Code | Description |
| ---- | ----------- |
| 201 | Successful Response |
| 405 | Invalid Input |

# /probe/{id}
## ***GET***

**Summary:** List Probe Details/Readings associated with id provided and within those associated with the account key

### HTTP Request
`***GET*** /probe/{id}`

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path | id of probe to retrieve | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Successful Response |

<!-- Converted with the swagger-to-slate https://github.com/lavkumarv/swagger-to-slate -->
