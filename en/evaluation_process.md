# Multiplicity

## Authorization

1. Sign in with the account
2. Click on [Credentials](www.multiplicityassess.com/accounts/api_credentials)
3. Create a new token

#### Notes

- Token will expire yearly
- Only account administrators can create or remove tokens
- _Method:_ Bearer Token

## Evaluation Process
### Search Process
**GET** `www.multiplicityassess.com/api/evaluation_processes`

##### Request
```cURL
curl --location --request GET 'multiplicityassess.com/api/evaluation_processes' \
--data '{
    "name_cont": "Tes"
}'
```


##### Response
```json
[
    {
        "name": "Test",
        "status": "Started",
        "sector": "-",
        "creation_date": "2023-03-09T15:43:08.085-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Test",
        "ideal_profile": true,
        "category": "Recruitment",
        "calculation": "Minimun",
        "group": {
            "id": 5,
            "name": "Recepcionista"
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "client",
                        "expected": "-"
                    },
                    {
                        "name": "innovation",
                        "expected": "-"
                    }
                ]
            },
            {
                "name": "Motivadores",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "professional",
                        "expected": "-"
                    },
                    {
                        "name": "autonomy",
                        "expected": "-"
                    },
                    {
                        "name": "identification",
                        "expected": "-"
                    },
                    {
                        "name": "belonging",
                        "expected": "-"
                    },
                    {
                        "name": "meaning",
                        "expected": "-"
                    },
                    {
                        "name": "relationships",
                        "expected": "-"
                    },
                    {
                        "name": "defy",
                        "expected": "-"
                    },
                    {
                        "name": "equity",
                        "expected": "-"
                    },
                    {
                        "name": "economic",
                        "expected": "-"
                    },
                    {
                        "name": "promotion",
                        "expected": "-"
                    },
                    {
                        "name": "trust",
                        "expected": "-"
                    },
                    {
                        "name": "trascendency",
                        "expected": "-"
                    }
                ]
            },
            {
                "name": "Razonamiento general",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "operaciones",
                        "expected": "-"
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": " ",
                "email": "robert.marcelino@resolvedigital.com",
                "user": null,
                "password": "3b8a74",
                "status": "started"
            },
            {
                "name": " ",
                "email": "robert.marcelino@outlook.com",
                "user": null,
                "password": "6df571",
                "status": "started"
            }
        ]
    },
    {
        "name": "Test",
        "status": "Incomplete",
        "sector": "-",
        "creation_date": "2023-08-30T09:14:56.036-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Test",
        "ideal_profile": false,
        "category": "Recruitment",
        "calculation": "Minimun",
        "group": {
            "id": 5,
            "name": "Recepcionista"
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "innovation",
                        "expected": "-"
                    },
                    {
                        "name": "client",
                        "expected": "-"
                    }
                ]
            },
            {
                "name": "Motivadores",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "equity",
                        "expected": "-"
                    },
                    {
                        "name": "trascendency",
                        "expected": "-"
                    },
                    {
                        "name": "trust",
                        "expected": "-"
                    },
                    {
                        "name": "meaning",
                        "expected": "-"
                    },
                    {
                        "name": "autonomy",
                        "expected": "-"
                    },
                    {
                        "name": "defy",
                        "expected": "-"
                    },
                    {
                        "name": "promotion",
                        "expected": "-"
                    },
                    {
                        "name": "professional",
                        "expected": "-"
                    },
                    {
                        "name": "economic",
                        "expected": "-"
                    },
                    {
                        "name": "identification",
                        "expected": "-"
                    },
                    {
                        "name": "relationships",
                        "expected": "-"
                    },
                    {
                        "name": "belonging",
                        "expected": "-"
                    }
                ]
            },
            {
                "name": "Razonamiento general",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "operaciones",
                        "expected": "-"
                    }
                ]
            }
        ],
        "participants": []
    },
    {
        "name": "Test proceso nuevo staging - 1",
        "status": "Started",
        "sector": "-",
        "creation_date": "2023-03-10T00:46:30.381-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Test",
        "ideal_profile": true,
        "category": "Recruitment",
        "calculation": "Minimun",
        "group": {
            "id": 3,
            "name": "Auxiliar"
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": true,
                "categories": [
                    {
                        "name": "initiative",
                        "expected": 4
                    },
                    {
                        "name": "planification",
                        "expected": 4
                    },
                    {
                        "name": "business",
                        "expected": 4
                    },
                    {
                        "name": "innovation",
                        "expected": 5
                    }
                ]
            },
            {
                "name": "Pensamiento analítico y sistémico",
                "ideal_profile": true,
                "categories": [
                    {
                        "name": "systemic_judgement",
                        "expected": 3
                    },
                    {
                        "name": "analytical_judgement",
                        "expected": 5
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": " ",
                "email": "robert.marcelino@resolvedigital.com",
                "user": null,
                "password": "e7d418",
                "status": "finished"
            }
        ]
    },
    {
        "name": "Test creacion de procesos nuevo flujo account -2",
        "status": "Incomplete",
        "sector": "-",
        "creation_date": "2023-03-10T12:17:47.660-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Test",
        "ideal_profile": true,
        "category": "Recruitment",
        "calculation": "Minimun",
        "group": {
            "id": 3,
            "name": "Auxiliar"
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": false,
                "categories": []
            },
            {
                "name": "Motivadores",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "defy",
                        "expected": "-"
                    },
                    {
                        "name": "autonomy",
                        "expected": "-"
                    },
                    {
                        "name": "trascendency",
                        "expected": "-"
                    },
                    {
                        "name": "economic",
                        "expected": "-"
                    },
                    {
                        "name": "trust",
                        "expected": "-"
                    },
                    {
                        "name": "equity",
                        "expected": "-"
                    },
                    {
                        "name": "relationships",
                        "expected": "-"
                    },
                    {
                        "name": "promotion",
                        "expected": "-"
                    },
                    {
                        "name": "identification",
                        "expected": "-"
                    },
                    {
                        "name": "meaning",
                        "expected": "-"
                    },
                    {
                        "name": "belonging",
                        "expected": "-"
                    },
                    {
                        "name": "professional",
                        "expected": "-"
                    }
                ]
            }
        ],
        "participants": []
    },
    {
        "name": "Test",
        "status": "Started",
        "sector": "-",
        "creation_date": "2023-03-09T08:57:58.752-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Test",
        "ideal_profile": true,
        "category": "Recruitment",
        "calculation": "Minimun",
        "group": {
            "id": 3,
            "name": "Auxiliar"
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "initiative",
                        "expected": "-"
                    },
                    {
                        "name": "client",
                        "expected": "-"
                    },
                    {
                        "name": "innovation",
                        "expected": "-"
                    }
                ]
            },
            {
                "name": "Motivadores",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "promotion",
                        "expected": "-"
                    },
                    {
                        "name": "trust",
                        "expected": "-"
                    },
                    {
                        "name": "autonomy",
                        "expected": "-"
                    },
                    {
                        "name": "professional",
                        "expected": "-"
                    },
                    {
                        "name": "economic",
                        "expected": "-"
                    },
                    {
                        "name": "equity",
                        "expected": "-"
                    },
                    {
                        "name": "belonging",
                        "expected": "-"
                    },
                    {
                        "name": "trascendency",
                        "expected": "-"
                    },
                    {
                        "name": "meaning",
                        "expected": "-"
                    },
                    {
                        "name": "identification",
                        "expected": "-"
                    },
                    {
                        "name": "defy",
                        "expected": "-"
                    },
                    {
                        "name": "relationships",
                        "expected": "-"
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": " ",
                "email": "rmarcelino@bluecoding.com",
                "user": null,
                "password": "decfda",
                "status": "finished"
            },
            {
                "name": " ",
                "email": "robert.marcelino@resolvedigital.com",
                "user": null,
                "password": "2ee24a",
                "status": "finished"
            }
        ]
    },
    {
        "name": "Test",
        "status": "Incomplete",
        "sector": "-",
        "creation_date": "2023-03-09T15:41:38.568-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Test",
        "ideal_profile": true,
        "category": "Recruitment",
        "calculation": "Minimun",
        "group": {
            "id": 5,
            "name": "Recepcionista"
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": false,
                "categories": []
            },
            {
                "name": "Razonamiento general",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "operaciones",
                        "expected": "-"
                    }
                ]
            }
        ],
        "participants": []
    },
    {
        "name": "Test Yudelka",
        "status": "Incomplete",
        "sector": "-",
        "creation_date": "2023-08-25T14:11:23.447-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Test",
        "ideal_profile": false,
        "category": "Recruitment",
        "calculation": "Minimun",
        "group": {
            "id": 3,
            "name": "Auxiliar"
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "innovation",
                        "expected": "-"
                    },
                    {
                        "name": "client",
                        "expected": "-"
                    },
                    {
                        "name": "teamwork",
                        "expected": "-"
                    },
                    {
                        "name": "tolerance",
                        "expected": "-"
                    },
                    {
                        "name": "initiative",
                        "expected": "-"
                    }
                ]
            },
            {
                "name": "Motivadores",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "equity",
                        "expected": "-"
                    },
                    {
                        "name": "trascendency",
                        "expected": "-"
                    },
                    {
                        "name": "trust",
                        "expected": "-"
                    },
                    {
                        "name": "meaning",
                        "expected": "-"
                    },
                    {
                        "name": "autonomy",
                        "expected": "-"
                    },
                    {
                        "name": "defy",
                        "expected": "-"
                    },
                    {
                        "name": "promotion",
                        "expected": "-"
                    },
                    {
                        "name": "professional",
                        "expected": "-"
                    },
                    {
                        "name": "economic",
                        "expected": "-"
                    },
                    {
                        "name": "identification",
                        "expected": "-"
                    },
                    {
                        "name": "relationships",
                        "expected": "-"
                    },
                    {
                        "name": "belonging",
                        "expected": "-"
                    }
                ]
            }
        ],
        "participants": []
    },
    {
        "name": "CSV TEST",
        "status": "Started",
        "sector": "-",
        "creation_date": "2017-02-10T16:48:46.547-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": true,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Pensamiento analítico y sistémico",
                "ideal_profile": true,
                "categories": [
                    {
                        "name": "systemic_judgement",
                        "expected": 0
                    },
                    {
                        "name": "analytical_judgement",
                        "expected": 0
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": "Robert Marcelino",
                "email": "robert.marcelino@outlook.com",
                "user": null,
                "password": null,
                "status": "started"
            },
            {
                "name": " ",
                "email": "eurzua@bluecoding.com",
                "user": null,
                "password": null,
                "status": "started"
            }
        ]
    },
    {
        "name": "Testing after deploy",
        "status": "Started",
        "sector": "-",
        "creation_date": "2017-06-10T00:18:02.493-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": true,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Razonamiento general",
                "ideal_profile": true,
                "categories": [
                    {
                        "name": "operaciones",
                        "expected": 0
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": "Marcelino Robert",
                "email": "rmarcelino@bluecoding.com",
                "user": null,
                "password": null,
                "status": "started"
            }
        ]
    },
    {
        "name": "testing 05-07-17",
        "status": "Incomplete",
        "sector": "-",
        "creation_date": "2017-07-05T21:10:04.766-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": false,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": false,
                "categories": []
            }
        ],
        "participants": []
    },
    {
        "name": "testing Jaime",
        "status": "Incomplete",
        "sector": "-",
        "creation_date": "2017-07-26T11:40:54.706-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": false,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": false,
                "categories": []
            }
        ],
        "participants": [
            {
                "name": "Marcelino Robert",
                "email": "rmarcelino@bluecoding.com",
                "user": null,
                "password": null,
                "status": "added"
            },
            {
                "name": " ",
                "email": "jvinas@bluecoding.com",
                "user": null,
                "password": null,
                "status": "added"
            },
            {
                "name": "Hemmat David",
                "email": "dhemmat@bluecoding.com",
                "user": null,
                "password": null,
                "status": "added"
            },
            {
                "name": " ",
                "email": "rmarcelino@ahs.do",
                "user": null,
                "password": null,
                "status": "added"
            },
            {
                "name": " ",
                "email": "test@bluecoding.com",
                "user": null,
                "password": null,
                "status": "added"
            }
        ]
    },
    {
        "name": "test",
        "status": "Incomplete",
        "sector": "-",
        "creation_date": "2017-11-03T09:48:51.458-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": true,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": true,
                "categories": [
                    {
                        "name": "negociation",
                        "expected": 4
                    },
                    {
                        "name": "initiative",
                        "expected": 4
                    },
                    {
                        "name": "people_management",
                        "expected": 4
                    },
                    {
                        "name": "business",
                        "expected": 4
                    },
                    {
                        "name": "tolerance",
                        "expected": 4
                    },
                    {
                        "name": "networking",
                        "expected": 4
                    },
                    {
                        "name": "innovation",
                        "expected": 4
                    },
                    {
                        "name": "sensitivity",
                        "expected": 4
                    },
                    {
                        "name": "flexibility",
                        "expected": 4
                    }
                ]
            },
            {
                "name": "Motivadores",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "defy",
                        "expected": "-"
                    },
                    {
                        "name": "promotion",
                        "expected": "-"
                    },
                    {
                        "name": "relationships",
                        "expected": "-"
                    },
                    {
                        "name": "economic",
                        "expected": "-"
                    },
                    {
                        "name": "belonging",
                        "expected": "-"
                    },
                    {
                        "name": "trascendency",
                        "expected": "-"
                    },
                    {
                        "name": "meaning",
                        "expected": "-"
                    },
                    {
                        "name": "identification",
                        "expected": "-"
                    },
                    {
                        "name": "autonomy",
                        "expected": "-"
                    },
                    {
                        "name": "professional",
                        "expected": "-"
                    },
                    {
                        "name": "equity",
                        "expected": "-"
                    },
                    {
                        "name": "trust",
                        "expected": "-"
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": " ",
                "email": "robert.marcelino@resolvedigital.com",
                "user": null,
                "password": "c28f1f",
                "status": "added"
            }
        ]
    },
    {
        "name": "test 04-11",
        "status": "Started",
        "sector": "-",
        "creation_date": "2017-04-11T15:29:35.702-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": false,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Pensamiento analítico y sistémico",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "systemic_judgement",
                        "expected": "-"
                    },
                    {
                        "name": "analytical_judgement",
                        "expected": "-"
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": " ",
                "email": "eurzua@bluecoding.com",
                "user": null,
                "password": null,
                "status": "started"
            }
        ]
    },
    {
        "name": "test invitation review",
        "status": "Started",
        "sector": "-",
        "creation_date": "2017-12-05T16:02:33.104-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": false,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Razonamiento general",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "operaciones",
                        "expected": "-"
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": "Marcelino Robert",
                "email": "rmarcelino@bluecoding.com",
                "user": null,
                "password": null,
                "status": "joined"
            },
            {
                "name": " ",
                "email": "test1@test.com",
                "user": null,
                "password": null,
                "status": "joined"
            },
            {
                "name": " ",
                "email": "test2@test.com",
                "user": null,
                "password": null,
                "status": "joined"
            }
        ]
    },
    {
        "name": "Test para duplicación (1)",
        "status": "Incomplete",
        "sector": "-",
        "creation_date": "2018-05-14T16:17:41.126-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": true,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": true,
                "categories": [
                    {
                        "name": "initiative",
                        "expected": 4
                    },
                    {
                        "name": "people_management",
                        "expected": 5
                    },
                    {
                        "name": "business",
                        "expected": 4
                    },
                    {
                        "name": "networking",
                        "expected": 3
                    },
                    {
                        "name": "innovation",
                        "expected": 3
                    }
                ]
            },
            {
                "name": "Motivadores",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "defy",
                        "expected": "-"
                    },
                    {
                        "name": "promotion",
                        "expected": "-"
                    },
                    {
                        "name": "economic",
                        "expected": "-"
                    },
                    {
                        "name": "meaning",
                        "expected": "-"
                    },
                    {
                        "name": "trascendency",
                        "expected": "-"
                    },
                    {
                        "name": "professional",
                        "expected": "-"
                    },
                    {
                        "name": "identification",
                        "expected": "-"
                    },
                    {
                        "name": "trust",
                        "expected": "-"
                    },
                    {
                        "name": "equity",
                        "expected": "-"
                    },
                    {
                        "name": "relationships",
                        "expected": "-"
                    },
                    {
                        "name": "autonomy",
                        "expected": "-"
                    },
                    {
                        "name": "belonging",
                        "expected": "-"
                    }
                ]
            }
        ],
        "participants": []
    },
    {
        "name": "test razonamiento (1)",
        "status": "Started",
        "sector": "-",
        "creation_date": "2018-06-01T13:04:26.739-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": false,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": false,
                "categories": []
            },
            {
                "name": "Razonamiento general",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "operaciones",
                        "expected": "-"
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": " ",
                "email": "robert.marcelino@resolvedigital.com",
                "user": null,
                "password": "9c2f7f",
                "status": "joined"
            },
            {
                "name": " ",
                "email": "eurzua@bluecoding.com",
                "user": null,
                "password": null,
                "status": "joined"
            }
        ]
    },
    {
        "name": "test razonamiento",
        "status": "Started",
        "sector": "-",
        "creation_date": "2017-12-14T12:06:43.208-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": false,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": false,
                "categories": []
            },
            {
                "name": "Razonamiento general",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "operaciones",
                        "expected": "-"
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": " ",
                "email": "eurzua@bluecoding.com",
                "user": null,
                "password": null,
                "status": "joined"
            }
        ]
    },
    {
        "name": "test cluster",
        "status": "Started",
        "sector": "-",
        "creation_date": "2018-09-27T11:04:32.494-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": true,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": true,
                "categories": [
                    {
                        "name": "sensitivity",
                        "expected": 4
                    },
                    {
                        "name": "negociation",
                        "expected": 5
                    },
                    {
                        "name": "tolerance",
                        "expected": 3
                    },
                    {
                        "name": "flexibility",
                        "expected": 4
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": "Marcelino Robert",
                "email": "rmarcelino@bluecoding.com",
                "user": null,
                "password": null,
                "status": "joined"
            },
            {
                "name": "Marcelino Robert",
                "email": "robert.marcelino.c@gmail.com",
                "user": null,
                "password": null,
                "status": "finished"
            }
        ]
    },
    {
        "name": "Test para duplicación (2)",
        "status": "Started",
        "sector": "-",
        "creation_date": "2018-05-15T13:37:59.600-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": true,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "flexibility",
                        "expected": "-"
                    },
                    {
                        "name": "tolerance",
                        "expected": "-"
                    },
                    {
                        "name": "negociation",
                        "expected": "-"
                    },
                    {
                        "name": "sensitivity",
                        "expected": "-"
                    }
                ]
            },
            {
                "name": "Motivadores",
                "ideal_profile": true,
                "categories": [
                    {
                        "name": "defy",
                        "expected": 4
                    },
                    {
                        "name": "promotion",
                        "expected": 2
                    },
                    {
                        "name": "economic",
                        "expected": 9
                    },
                    {
                        "name": "meaning",
                        "expected": 5
                    },
                    {
                        "name": "trascendency",
                        "expected": 7
                    },
                    {
                        "name": "professional",
                        "expected": 10
                    },
                    {
                        "name": "identification",
                        "expected": 3
                    },
                    {
                        "name": "trust",
                        "expected": 1
                    },
                    {
                        "name": "equity",
                        "expected": 11
                    },
                    {
                        "name": "relationships",
                        "expected": 6
                    },
                    {
                        "name": "autonomy",
                        "expected": 8
                    },
                    {
                        "name": "belonging",
                        "expected": 0
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": " ",
                "email": "development@bluecoding.com",
                "user": null,
                "password": null,
                "status": "added"
            },
            {
                "name": " ",
                "email": "r.marcelino.camilo@gmail.com",
                "user": null,
                "password": null,
                "status": "added"
            },
            {
                "name": "Marcelino Robert",
                "email": "robert.marcelino.c@gmail.com",
                "user": null,
                "password": null,
                "status": "joined"
            },
            {
                "name": "Marcelino Robert",
                "email": "rmarcelino@bluecoding.com",
                "user": null,
                "password": null,
                "status": "joined"
            }
        ]
    },
    {
        "name": "test completivo sin ideal competencias iguales",
        "status": "Started",
        "sector": "-",
        "creation_date": "2018-12-27T16:27:59.385-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": true,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": true,
                "categories": [
                    {
                        "name": "negociation",
                        "expected": 3
                    },
                    {
                        "name": "impact",
                        "expected": 3
                    },
                    {
                        "name": "business",
                        "expected": 3
                    },
                    {
                        "name": "client",
                        "expected": 3
                    },
                    {
                        "name": "compromise",
                        "expected": 3
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": "Marcelino Robert",
                "email": "rmarcelino@bluecoding.com",
                "user": null,
                "password": null,
                "status": "finished"
            }
        ]
    },
    {
        "name": "test clusters marcados al iniciar",
        "status": "Started",
        "sector": "-",
        "creation_date": "2018-12-28T10:01:56.511-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": true,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": true,
                "categories": [
                    {
                        "name": "initiative",
                        "expected": 4
                    },
                    {
                        "name": "people_management",
                        "expected": 5
                    },
                    {
                        "name": "business",
                        "expected": 5
                    },
                    {
                        "name": "networking",
                        "expected": 4
                    },
                    {
                        "name": "innovation",
                        "expected": 5
                    }
                ]
            }
        ],
        "participants": [
            {
                "name": "Marcelino Robert",
                "email": "rmarcelino@bluecoding.com",
                "user": null,
                "password": null,
                "status": "finished"
            }
        ]
    },
    {
        "name": "Test para duplicación",
        "status": "Incomplete",
        "sector": "-",
        "creation_date": "2018-05-14T15:31:07.264-04:00",
        "start_at": null,
        "end_at": null,
        "invitation": "Invitation",
        "position": "Old",
        "ideal_profile": true,
        "category": "All",
        "calculation": "Minimun",
        "group": {
            "id": 1,
            "name": ""
        },
        "surveys": [
            {
                "name": "Competencias",
                "ideal_profile": false,
                "categories": [
                    {
                        "name": "flexibility",
                        "expected": "-"
                    },
                    {
                        "name": "tolerance",
                        "expected": "-"
                    },
                    {
                        "name": "negociation",
                        "expected": "-"
                    },
                    {
                        "name": "sensitivity",
                        "expected": "-"
                    }
                ]
            },
            {
                "name": "Motivadores",
                "ideal_profile": true,
                "categories": [
                    {
                        "name": "belonging",
                        "expected": 0
                    },
                    {
                        "name": "autonomy",
                        "expected": 8
                    },
                    {
                        "name": "relationships",
                        "expected": 6
                    },
                    {
                        "name": "equity",
                        "expected": 11
                    },
                    {
                        "name": "trust",
                        "expected": 1
                    },
                    {
                        "name": "identification",
                        "expected": 3
                    },
                    {
                        "name": "professional",
                        "expected": 10
                    },
                    {
                        "name": "trascendency",
                        "expected": 7
                    },
                    {
                        "name": "meaning",
                        "expected": 5
                    },
                    {
                        "name": "economic",
                        "expected": 9
                    },
                    {
                        "name": "promotion",
                        "expected": 2
                    },
                    {
                        "name": "defy",
                        "expected": 4
                    }
                ]
            }
        ],
        "participants": []
    }
]
```
### Create Process
Some rules regarding the configuration of processes:
  - Processes with operations type tests are basic and cannot be used in combination with skills. and vice versa.
  - If the skills test has an ideal profile, skills must also have an ideal profile.
  - The process must be configured correctly and contain at least one participant to be able to start.
#### With less arguments
The endpoint is designed to create a new evaluation process including surveys.

##### Request

**POST** `www.multiplicityassess.com/api/evaluation_processes`

```cURL
curl --location 'multiplicityassess.com/api/evaluation_processes' \
--data '{
  "evaluation_process": {
    "name" : "API Test 1",
    "category" : "all",
    "profile_evaluation_method" : "minimun",
    "position" : "Test",
    "occupational_group_id" : 1,
    "invitation_method" : "invitation"
  }
}'
```

##### Response

```json
{
  "message": "Process created successfully",
  "status": "created",
  "process": {
    "name": "API Test 1",
    "status": "No empezado",
    "calculation_method": "minimun",
    "start_at": null,
    "end_at": null,
    "invitation_mehtod": "invitation",
    "occupational_group": {
      "id": 1,
      "name": "Test"
    }
  }
}
```

#### With Ideal profile

##### Request
```cURL
curl --location 'multiplicityassess.com/api/evaluation_processes' \
--data '{
  "evaluation_process": {
    "name" : "API Test 1",
    "category" : "all",
    "profile_evaluation_method" : "minimun",
    "position" : "Test",
    "occupational_group_id" : 1,
    "invitation_method" : "invitation",
    "surveys" : {
      "competences" : {
        "flexibility": 3,
        "compromise" : 5,
        "innovation" : 4,
        "client" : 4,
        "teamwork": 3
      }
    }
  }
}'
```

##### Response
```json
{
  "message": "Process created successfully",
  "status": "created",
  "process": {
    "name": "API Test 1",
    "status": "No empezado",
    "calculation_method": "minimun",
    "start_at": null,
    "end_at": null,
    "invitation_mehtod": "invitation",
    "occupational_group": {
      "name": "",
      "id": 1
    },
    "surveys": [
      {
        "competences": [
          {
            "name": "teamwork",
            "ideal_profile": 3
          },
          {
            "name": "client",
            "ideal_profile": 4
          },
          {
            "name": "innovation",
            "ideal_profile": 4
          },
          {
            "name": "compromise",
            "ideal_profile": 5
          },
          {
            "name": "flexibility",
            "ideal_profile": 3
          }
        ]
      }
    ]
  }
}
```

#### Bad request | Missing position
Any of  the basic required fields missing should return an error message
##### Request
```cURL
curl --location 'multiplicityassess.com/api/evaluation_processes' \
--data '{
    "evaluation_process": {
        "name" : "API Test 1",
        "category" : "all",
        // "profile_evaluation_method" : "minimun",
        "position" : "Test",
        "occupational_group_id" : 1,
        "invitation_method" : "invitation"
    }
}'
```
##### Response
```json
{
  "message": "Process not created",
  "errors": {
    "position": [
      "Debe indicar cual es la posición a evaluar."
    ]
  }
}
```
### Add Participants
#### With Email
**POST** `multiplicityassess.com/api/evaluation_processes/api-test-1/invite`

##### Request
```cURL
curl --location 'multiplicityassess.com/api/evaluation_processes/api-test-1/invite' \
--data-raw '{
    "participant" : {
        "email" : "robert.marcelino+5@resolvedigital.com"
    }
}'
```
##### Response
```json
{
  "email": "robert.marcelino+5@resolvedigital.com",
  "username": null,
  "first_name": null,
  "last_name": null,
  "password": "cda73e",
  "status": "added",
  "invitations": 0,
  "process": {
    "id": 7946,
    "name": "API Test 1"
  }
}
```
#### With Username
##### Request
```cURL
curl --location 'multiplicityassess.com/api/evaluation_processes/api-test-1/invite' \
--data-raw '{
    "participant" : {
        "username" : "rmarcelino"
    }
}'
```
##### Response
```json
{
  "email": null,
  "username": "rmarcelino",
  "first_name": null,
  "last_name": null,
  "password": "cda73e",
  "status": "added",
  "invitations": 0,
  "process": {
    "id": 7946,
    "name": "API Test 1"
  }
}
```
#### Bad Request
##### Request
```cURL
  curl --location 'multiplicityassess.com/api/evaluation_processes/api-test-1/invite'
```
##### Response
```json
{
  "message": "param is missing or the value is empty: participant"
}
```
### Start process
**GET**