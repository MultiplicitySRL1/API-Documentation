# Multiplicity

## Authorization
1. Sign in with the account
2. Click on [Credentials](www.multiplicityassess.com/accounts/api_credentials)
3. Create a new token

#### Notes
- Token will expire yearly
- Only account administrators can create or remove tokens
- *Method:* Bearer Token

## Tools
### Occupational Group
The endpoint is designed to provide users with information about different occupational groups, including a list of professions. This endpoint acts as a resource for retrieving comprehensive information related to occupational groups.
#### Regular Request
##### Request
```cURL
curl --location 'www.multiplicityassess.com/api/occupational_groups'
```

##### Response
```json
[
    {
        "id": "cajero",
        "name": "Cajero"
    },
    {
        "id": "supervisores",
        "name": "Supervisores"
    },
    {
        "id": "encargados",
        "name": "Encargados"
    },
    {
        "id": "gerentes-jr",
        "name": "Gerentes Jr"
    },
    {
        "id": "vicepresidentes",
        "name": "Vicepresidentes"
    },
    {
        "id": "directores",
        "name": "Directores"
    }
]
```

#### Search by name
##### Request
```cURL
curl --location '192.168.5.211:3001/api/occupational_groups?name_cont=supervisores'

```

##### Response
```json
[
    {
        "id": "supervisores",
        "name": "Supervisores"
    }
]
```