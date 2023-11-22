# Multiplicity

## Authorization
1. Sign in with the account
2. Click on [Credentials](www.multiplicityassess.com/accounts/api_credentials)
3. Create a new token

#### Notes
- Token will expire yearly
- Only account administrators can create or remove tokens
- *Method:* Bearer Token

## Reports

The endpoint is designed to provide users with information about different Reports.

### Regular Request
#### Request
```cURL
curl --location 'www.multiplicityassess.com/api/reports/participations/11644/standard'
```

#### Response
```json
{
    "Name": "Marcelino Robert",
    "Status": "Finalizado",
    "Invitations Count": 0,
    "Process": {
        "Id": "proceso-prueba-minerd",
        "Name": "Proceso Prueba MINERD",
        "Sector": "Educación, Formación",
        "Position": "old",
        "Occupational Group": "",
        "Category": "all",
        "Invitation By": "Invitation",
        "Pruebas": {
            "Competencias": {
                "Name": "Competencias",
                "Ideal Profile": true
            },
            "Motivadores": {
                "Name": "Motivadores",
                "Ideal Profile": true
            },
            "Pensamiento analítico y sistémico": {
                "Name": "Pensamiento analítico y sistémico",
                "Ideal Profile": true
            }
        }
    },
    "Results": {
        "Competencias": {
            "Profile Adjustment": "53%",
            "categories": {
                "sensitivity": {
                    "Expected Score": 3,
                    "Expected Definition": "Maneja con tacto las reacciones emocionales de otros.Manifiesta de forma clara empatía aunque no esté de acuerdo con las conductas de los otros.Trata de ver las cosas desde el punto de vista de otros para entender sus reacciones.Prevé las posibles reacciones de otros antes sus acciones.",
                    "Description": "Muestra una forma de relacionarse considerada comprensiva y empatica, escucha activamente y es receptivo a los sentimientos de los demás.",
                    "score": 4,
                    "Definition": "Anticipa las acciones de otros ante sus acciones y actúa en consecuencia.Tiene en cuenta las reacciones emocionales o los sentimientos de otros antes de tomar una decisión.Es capaz de detectar reacciones emocionales no manifiestas o sentimientos ocultos en otros.Consigue que los demás confíen en él/ella, y le externen sus preocupaciones o dificultades."
                },
                "negociation": {
                    "Expected Score": 3,
                    "Expected Definition": "Explora distintas posibilidades de acuerdo.Modifica su estrategia en función de la respuesta de su interlocutor.Presenta claramente las ventajas de su posición.Tiene claro interés por alcanzar un acuerdo, aunque éste sea provisional.Mantiene un equilibrio entre la defensa de sus intereses y el respeto por los del otro.",
                    "Description": "Reconoce los objetivos de las diferentes partes. Negocia soluciones mutuamente favorables mediante el compromiso, y genera situaciones “ganar-ganar”.",
                    "score": 1,
                    "Definition": "Tiene disposición para llegar a un acuerdo satisfactorio.Defiende su interés sin atropellar a la otra parte."
                },
                "tolerance": {
                    "Expected Score": 3,
                    "Expected Definition": "Mantiene la calma en situaciones de tensión media-alta. (Incidencias, errores propios o ajenos o urgencias frecuentes).Ve las situaciones tensas o imprevistas con perspectiva y no les da una importancia exagerada.El nivel de su rendimiento no se reduce en situaciones de presión media o media-alta. Mantiene el control sobre su comportamiento (lo que hace y dice es lo que conscientemente quiere decir y hacer) ante situaciones inesperadas.",
                    "Description": "Mantiene una actitud calmada, controlada y positiva bajo presión, manteniéndose centrado en la tarea.",
                    "score": 1,
                    "Definition": "Muestra calma en aquellas situaciones que conoce bien y en las cuales la tensión es baja.En situaciones conocidas o habituales actúa con prudencia.Su desempeño es más bajo en situaciones de mucha exigencia."
                },
                "flexibility": {
                    "Expected Score": 3,
                    "Expected Definition": "Se adapta muy rápidamente a nuevas situaciones, sin necesidad de que la organización realice ningún tipo de esfuerzo extra para que lo haga.Se adapta a tratar con distintos tipos de personas.Muestra opiniones y conductas positivas ante el cambio.Integra bien y rápidamente nueva información.Asume nuevos roles con facilidad.",
                    "Description": "Se adapta fácilmente a nuevas situaciones y formas de trabajar. Es receptivo a los cambios y muestra voluntad por adaptarse a ellos de forma efectiva.",
                    "score": 2,
                    "Definition": "Se adapta con facilidad a nuevas situaciones una vez las ha entendido y asumidoSe mueve con facilidad en ambientes ligeramente distintos al suyo."
                }
            }
        },
        "Motivadores": {
            "equity": {
                "Description": "Igualdad de oportunidades y posibilidades, trato justo.",
                "Expected": 11,
                "score": 3,
                "Definition": "Valora en cierta medida la equidad e igualdad de oportunidades dentro de la institución."
            },
            "professional": {
                "Description": "Status, consideración profesional, premios o reconocimientos no materiales.",
                "Expected": 10,
                "score": 3,
                "Definition": "Motivación media hacia premios, consideraciones o reconocimientos no materiales de su trabajo."
            },
            "economic": {
                "Description": "Dinero u otro tipo de reconocimiento material.",
                "Expected": 9,
                "score": 4,
                "Definition": "Muestra alto interés por la recompensa económica y material."
            },
            "autonomy": {
                "Description": "Independencia a la hora de gestionar el trabajo.",
                "Expected": 8,
                "score": 2,
                "Definition": "No da demasiada importancia a tener altos niveles de supervisión, aunque valora cierto nivel de autonomía en su trabajo."
            },
            "trascendency": {
                "Description": "Responsabilidad social y aportación a la sociedad.",
                "Expected": 7,
                "score": 2,
                "Definition": "Considera la responsabilidad social y la aportación de la institución a la sociedad un valor de escasa importancia."
            },
            "relationships": {
                "Description": "Comunicación fluida y clara con otras personas y/o departamentos.",
                "Expected": 6,
                "score": 3,
                "Definition": "La comunicación y las relaciones fluidas con otras personas y/o departamentos tienen una influencia media en su motivación."
            },
            "meaning": {
                "Description": "Trabajo significativo, donde puede verse claramente lo que se aporta a la organización.",
                "Expected": 5,
                "score": 4,
                "Definition": "El hacer un trabajo con un sentido claro o donde se vea claramente su importancia para la institución no es un valor significativo para el participante."
            },
            "defy": {
                "Description": "Trabajo retador, que pone a prueba nuestra capacidad.",
                "Expected": 4,
                "score": 2,
                "Definition": "El trabajo desafiante o retador es un factor que influye poco en sus niveles de motivación."
            },
            "identification": {
                "Description": "Sintonía entre mis objetivos y los objetivos de la institución.",
                "Expected": 3,
                "score": 3,
                "Definition": "La sintonía con los objetivos de la institución es un aspecto de mediana relevancia."
            },
            "promotion": {
                "Description": "Crecimiento vertical en el organigrama, mayor poder.",
                "Expected": 2,
                "score": 3,
                "Definition": "Se siente medianamente motivado por las posibilidades de promoción y/o alcanzar puestos de mayor poder."
            },
            "trust": {
                "Description": "Asertividad, posibilidad de hablar honesta y sinceramente.",
                "Expected": 1,
                "score": 2,
                "Definition": "Las relaciones honestas y de confianza dentro de la empresa son un elemento de poca importancia para él/ella."
            },
            "belonging": {
                "Description": "Integración en un equipo de forma consolidada.",
                "Expected": 0,
                "score": 4,
                "Definition": "La integración en grupos y/o equipos es un aspecto de alta prioridad."
            }
        },
        "Pensamiento analítico y sistémico": {
            "Profile Adjustment": "25%",
            "categories": {
                "systemic_judgement": {
                    "Expected Score": 3,
                    "Expected Definition": "Comprende en términos aceptables las relaciones entre los elementos de un sistema complejo.Es capaz de entender y anticipar los efectos que un cambio en un elemento del sistema tendrá sobre otros en problemas de complejidad media.Tiene una visión global aceptable de los problemas en situaciones de complejidad media.",
                    "Description": "Capacidad de solucionar problemas por medio de la percepción y comprensión de sistemas y elementos interrelacionados entre sí de una forma global, detectando las consecuencias que las interacciones entre los elementos tienen sobre el sistema como un todo.",
                    "score": 1,
                    "Definition": "Comprende las relaciones básicas entre los elementos de un sistema sencillo.Tiene una visión global de los problemas en situaciones sencillas o en las que no intervienen muchos elementos."
                },
                "analytical_judgement": {
                    "Expected Score": 3,
                    "Expected Definition": "Reúne y analiza información de complejidad media, estableciendo relaciones lógicas entre las partes de un problema.Maneja bien cantidades de información elevadas.Es capaz de reconocer vínculos causales de complejidad media ante un problema.Realiza análisis elaborados y resuelve problemas de complejidad media o media-alta.",
                    "Description": "Capacidad de solucionar problemas analizando sus partes constitutivas, integrando información dispersa y/o inconexa, y distinguiendo lo relevante de lo irrelevante.",
                    "score": 1,
                    "Definition": "Reúne y analiza información de baja complejidad.Detecta relaciones evidentes entre las partes de un problema.Maneja bien pequeñas cantidades de información.Es capaz de reconocer vínculos causales sencillos ante los problemas.Realiza análisis sencillos y resuelve problemas de poca complejidad."
                }
            }
        }
    }
}
```

### Regular Request (Basic Report)
#### Request
```cURL
curl --location 'www.multiplicityassess.com/api/reports/participations/11954/standard'
```

#### Response
```json
{
    "Name": " ",
    "Status": "Finalizado",
    "Invitations Count": 0,
    "Process": {
        "Id": "test-1301f4eb-4340-45b2-b34a-d2f61bedf6ae",
        "Name": "Test",
        "Sector": null,
        "Position": "Test",
        "Occupational Group": "Auxiliar",
        "Category": "recruitment",
        "Invitation By": "Invitation",
        "Pruebas": {
            "Motivadores": {
                "Name": "Motivadores",
                "Ideal Profile": false
            },
            "Competencias": {
                "Name": "Competencias",
                "Ideal Profile": false
            }
        }
    },
    "Results": {
        "Competencias": {
            "Average": 4,
            "categories": {
                "initiative": {
                    "Description": "Busca activamente oportunidades y actúa ante las mismas, sin necesidad de que otros lo muevan, mostrando una disposición a actuar de manera proactiva.",
                    "score": 5,
                    "Definition": "Identifica oportunidades que pasarían desapercibidas a otras personas.Anticipa posibles problemas a todos los niveles y a largo plazo, y actúa en consecuencia.Busca constantemente la forma de asumir mayores responsabilidades."
                },
                "client": {
                    "Description": "Identifica y comprende las necesidades del cliente. Se centra en satisfacer esas necesidades y asegurar tanto su satisfacción como una relación a largo plazo.",
                    "score": 4,
                    "Definition": "Se convierte en un asesor del cliente.Descubre nuevas formas de añadir valor al cliente.Adecua los productos o servicios disponibles a las necesidades del cliente.Busca nuevas formas de mejorar el servicio y la satisfacción del cliente."
                },
                "innovation": {
                    "Description": "Propone ideas nuevas y originales, así como enfoques novedosos y/o soluciones innovadoras. Ve más allá de los enfoques convencionales y de los métodos establecidos.",
                    "score": 4,
                    "Definition": "Involucra a otros miembros de su equipo en la búsqueda de nuevas soluciones.Busca de forma constante nuevos enfoques y modos de trabajo, más allá de mejorar lo existente.Propone mejoras estructurales o de concepto a lo ya existente.Genera nuevas alternativas (de mercado, de proceso, de servicio etc).Utiliza técnicas de generación de ideas."
                }
            }
        },
        "Motivadores": {
            "promotion": {
                "Description": "Crecimiento vertical en el organigrama, mayor poder.",
                "score": 2,
                "Definition": "Se siente poco motivado por las posibilidades de promoción y/o alcanzar puestos de mayor poder."
            },
            "trust": {
                "Description": "Asertividad, posibilidad de hablar honesta y sinceramente.",
                "score": 5,
                "Definition": "Las relaciones honestas y de confianza dentro de la empresa son un elemento de la máxima importancia para él/ella."
            },
            "autonomy": {
                "Description": "Independencia a la hora de gestionar el trabajo.",
                "score": 4,
                "Definition": "Es importante para él/ella poder realizar su trabajo con autonomía e independencia."
            },
            "professional": {
                "Description": "Status, consideración profesional, premios o reconocimientos no materiales.",
                "score": 1,
                "Definition": "Muy baja motivación hacia premios, consideraciones o reconocimientos no materiales de su trabajo."
            },
            "economic": {
                "Description": "Dinero u otro tipo de reconocimiento material.",
                "score": 1,
                "Definition": "Muestra muy escaso interés por la recompensa económica y material."
            },
            "equity": {
                "Description": "Igualdad de oportunidades y posibilidades, trato justo.",
                "score": 5,
                "Definition": "La equidad e igualdad de oportunidades dentro de la institución es un factor crítico para él/ella."
            },
            "belonging": {
                "Description": "Integración en un equipo de forma consolidada.",
                "score": 1,
                "Definition": "La integración en grupos y/o equipos es un aspecto de muy baja prioridad."
            },
            "trascendency": {
                "Description": "Responsabilidad social y aportación a la sociedad.",
                "score": 5,
                "Definition": "Considera la responsabilidad social y la aportación de la institución a la sociedad un valor de la máxima importancia."
            },
            "meaning": {
                "Description": "Trabajo significativo, donde puede verse claramente lo que se aporta a la organización.",
                "score": 4,
                "Definition": "El hacer un trabajo con un sentido claro o donde se vea claramente su importancia para la institución no es un valor significativo para el participante."
            },
            "identification": {
                "Description": "Sintonía entre mis objetivos y los objetivos de la institución.",
                "score": 3,
                "Definition": "La sintonía con los objetivos de la institución es un aspecto de mediana relevancia."
            },
            "defy": {
                "Description": "Trabajo retador, que pone a prueba nuestra capacidad.",
                "score": 3,
                "Definition": "El trabajo desafiante o retador es un factor que influye en cierta medida en sus niveles de motivación."
            },
            "relationships": {
                "Description": "Comunicación fluida y clara con otras personas y/o departamentos.",
                "score": 2,
                "Definition": "La comunicación y las relaciones fluidas con otras personas y/o departamentos tienen baja influencia en su motivación."
            }
        }
    }
}
```

### Without Ideal Profile version
#### Request
```cURL

```

#### Response
```json

```