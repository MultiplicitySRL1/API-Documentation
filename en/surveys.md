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
### Surveys
The endpoint is designed to provide users with information about different types of survey. This endpoint acts as a resource for retrieving comprehensive information related to survey.
#### Regular Request
##### Request
```cURL
curl --location 'www.multiplicityassess.com/api/surveys'
```

##### Response
```json
[
    {
        "id": "competences",
        "name": "competences",
        "categories": [
            {
                "id": "compromise",
                "name": "compromise"
            },
            {
                "id": "innovation",
                "name": "innovation"
            },
            {
                "id": "client",
                "name": "client"
            },
            {
                "id": "teamwork",
                "name": "teamwork"
            },
            {
                "id": "networking",
                "name": "networking"
            },
            {
                "id": "tolerance",
                "name": "tolerance"
            },
            {
                "id": "business",
                "name": "business"
            },
            {
                "id": "impact",
                "name": "impact"
            },
            {
                "id": "people_management",
                "name": "people_management"
            },
            {
                "id": "planification",
                "name": "planification"
            },
            {
                "id": "initiative",
                "name": "initiative"
            },
            {
                "id": "results",
                "name": "results"
            },
            {
                "id": "negociation",
                "name": "negociation"
            },
            {
                "id": "sensitivity",
                "name": "sensitivity"
            },
            {
                "id": "flexibility",
                "name": "flexibility"
            }
        ]
    },
    {
        "id": "operational",
        "name": "operational",
        "categories": [
            {
                "id": "operaciones",
                "name": "operaciones"
            }
        ]
    },
    {
        "id": "skills",
        "name": "skills",
        "categories": [
            {
                "id": "analytical_judgement",
                "name": "analytical_judgement"
            },
            {
                "id": "systemic_judgement",
                "name": "systemic_judgement"
            }
        ]
    },
    {
        "id": "motivational",
        "name": "motivational",
        "categories": [
            {
                "id": "belonging",
                "name": "belonging"
            },
            {
                "id": "relationships",
                "name": "relationships"
            },
            {
                "id": "identification",
                "name": "identification"
            },
            {
                "id": "economic",
                "name": "economic"
            },
            {
                "id": "professional",
                "name": "professional"
            },
            {
                "id": "promotion",
                "name": "promotion"
            },
            {
                "id": "defy",
                "name": "defy"
            },
            {
                "id": "autonomy",
                "name": "autonomy"
            },
            {
                "id": "meaning",
                "name": "meaning"
            },
            {
                "id": "trust",
                "name": "trust"
            },
            {
                "id": "trascendency",
                "name": "trascendency"
            },
            {
                "id": "equity",
                "name": "equity"
            }
        ]
    }
]
```

#### Search by name
##### Request
```cURL
curl --location 'www.multiplicityassess.com/api/surveys/competences'

```

##### Response
```json
{
    "id": "competences",
    "name": "competences",
    "categories": [
        {
            "id": "compromise",
            "name": "compromise"
        },
        {
            "id": "innovation",
            "name": "innovation"
        },
        {
            "id": "client",
            "name": "client"
        },
        {
            "id": "teamwork",
            "name": "teamwork"
        },
        {
            "id": "networking",
            "name": "networking"
        },
        {
            "id": "tolerance",
            "name": "tolerance"
        },
        {
            "id": "business",
            "name": "business"
        },
        {
            "id": "impact",
            "name": "impact"
        },
        {
            "id": "people_management",
            "name": "people_management"
        },
        {
            "id": "planification",
            "name": "planification"
        },
        {
            "id": "initiative",
            "name": "initiative"
        },
        {
            "id": "results",
            "name": "results"
        },
        {
            "id": "negociation",
            "name": "negociation"
        },
        {
            "id": "sensitivity",
            "name": "sensitivity"
        },
        {
            "id": "flexibility",
            "name": "flexibility"
        }
    ]
}
```