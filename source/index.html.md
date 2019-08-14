--- 

title: Wirex Business OpenApi 

language_tabs: 
   - shell 

toc_footers: 
   - <a href='#'>Sign Up for a Developer Key</a> 
   - <a href='https://github.com/lavkumarv'>Documentation Powered by lav</a> 

includes: 
   - errors 

search: true 

--- 

# Introduction 

**Version:** v1 

# Authentication 

|basic|*Basic*|
|---|---| 

|apiKey|*API Key*|
|---|---| 

# /SSO/.WELL-KNOWN/OPENID-CONFIGURATION/JWKS
## ***GET*** 

### HTTP Request 
`***GET*** /sso/.well-known/openid-configuration/jwks` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /SSO/.WELL-KNOWN/OPENID-CONFIGURATION
## ***GET*** 

### HTTP Request 
`***GET*** /sso/.well-known/openid-configuration` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /SSO/CONNECT/TOKEN
## ***POST*** 

### HTTP Request 
`***POST*** /sso/connect/token` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| client_id | formData |  | Yes | string |
| client_secret | formData |  | Yes | string |
| grant_type | formData |  | Yes | string |
| username | formData |  | No | string |
| password | formData |  | No | string |
| device_id | formData |  | Yes | string |
| device_name | formData |  | Yes | string |
| scope | formData |  | No | string |
| two_factor_code | formData |  | No | string |
| authorization_context | formData |  | No | string |
| code | formData |  | No | string |
| refresh_token | formData |  | No | string |
| redirect_uri | formData |  | No | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /SSO/CONNECT/REVOCATION
## ***POST*** 

### HTTP Request 
`***POST*** /sso/connect/revocation` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| token | formData |  | Yes | string |
| token_type_hint | formData |  | Yes | string |
| client_id | formData |  | Yes | string |
| client_secret | formData |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /BUSINESS/DICTIONARIES/{DICTIONARYTYPE}
## ***GET*** 

### HTTP Request 
`***GET*** /business/dictionaries/{dictionaryType}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| dictionaryType | path |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 404 | Not Found |

# /BUSINESS/EMPLOYEES
## ***GET*** 

### HTTP Request 
`***GET*** /business/employees` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /BUSINESS/EMPLOYEES/{ID}
## ***GET*** 

### HTTP Request 
`***GET*** /business/employees/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | string (uuid) |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /BUSINESS/PUBLIC-COMPANIES
## ***GET*** 

### HTTP Request 
`***GET*** /business/public-companies` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| CompanyName | query |  | No | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /BUSINESS/PUBLIC-COMPANIES/{ID}
## ***GET*** 

### HTTP Request 
`***GET*** /business/public-companies/{id}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | string (uuid) |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /BUSINESS/PUBLIC-COMPANIES/{ID}/PROFILE
## ***GET*** 

### HTTP Request 
`***GET*** /business/public-companies/{id}/profile` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | string (uuid) |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /BUSINESS/ROLES/{ROLEID}
## ***GET*** 

### HTTP Request 
`***GET*** /business/roles/{roleId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| roleId | path |  | Yes | string (uuid) |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /BUSINESS/ROLES
## ***GET*** 

### HTTP Request 
`***GET*** /business/roles` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /BUSINESS/ROLES/{ROLEID}/POLICY
## ***GET*** 

### HTTP Request 
`***GET*** /business/roles/{roleId}/policy` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| roleId | path |  | Yes | string (uuid) |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /BUSINESS/USER-COMPANIES
## ***GET*** 

### HTTP Request 
`***GET*** /business/user-companies` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

# /BUSINESS/USERS/INVITES
## ***GET*** 

### HTTP Request 
`***GET*** /business/users/invites` 

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |

<!-- Converted with the swagger-to-slate https://github.com/lavkumarv/swagger-to-slate -->
