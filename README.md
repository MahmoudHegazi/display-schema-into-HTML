# display-schema-into-HTML

```HTML
{
    "data": {
        "__schema": {
            "queryType": {
                "name": "Query"
            },
            "mutationType": {
                "name": "Mutation"
            },
            "subscriptionType": null,
            "types": [
                {
                    "kind": "OBJECT",
                    "name": "Query",
                    "description": "all queries for Dog table  and also if other tables",
                    "fields": [
                        {
                            "name": "getAllDogs",
                            "description": "return all dogs data",
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "LIST",
                                    "name": null,
                                    "ofType": {
                                        "kind": "OBJECT",
                                        "name": "Dog",
                                        "ofType": null
                                    }
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "findDogBreeds",
                            "description": "",
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "LIST",
                                    "name": null,
                                    "ofType": {
                                        "kind": "SCALAR",
                                        "name": "String",
                                        "ofType": null
                                    }
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "findDogById",
                            "description": "",
                            "args": [
                                {
                                    "name": "id",
                                    "description": "",
                                    "type": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "SCALAR",
                                            "name": "ID",
                                            "ofType": null
                                        }
                                    },
                                    "defaultValue": null
                                }
                            ],
                            "type": {
                                "kind": "OBJECT",
                                "name": "Dog",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "findDogBreedById",
                            "description": "",
                            "args": [
                                {
                                    "name": "id",
                                    "description": "",
                                    "type": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "SCALAR",
                                            "name": "ID",
                                            "ofType": null
                                        }
                                    },
                                    "defaultValue": null
                                }
                            ],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "String",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "findAllDogNames",
                            "description": "",
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "LIST",
                                    "name": null,
                                    "ofType": {
                                        "kind": "SCALAR",
                                        "name": "String",
                                        "ofType": null
                                    }
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        }
                    ],
                    "inputFields": null,
                    "interfaces": [],
                    "enumValues": null,
                    "possibleTypes": null
                },
                {
                    "kind": "SCALAR",
                    "name": "String",
                    "description": "Built-in String",
                    "fields": null,
                    "inputFields": null,
                    "interfaces": null,
                    "enumValues": null,
                    "possibleTypes": null
                },
                {
                    "kind": "SCALAR",
                    "name": "ID",
                    "description": "Built-in ID",
                    "fields": null,
                    "inputFields": null,
                    "interfaces": null,
                    "enumValues": null,
                    "possibleTypes": null
                },
                {
                    "kind": "OBJECT",
                    "name": "Mutation",
                    "description": "all mutations for the Dog table and also if other tables",
                    "fields": [
                        {
                            "name": "newDog",
                            "description": "",
                            "args": [
                                {
                                    "name": "name",
                                    "description": "",
                                    "type": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "SCALAR",
                                            "name": "String",
                                            "ofType": null
                                        }
                                    },
                                    "defaultValue": null
                                },
                                {
                                    "name": "modal",
                                    "description": "",
                                    "type": {
                                        "kind": "SCALAR",
                                        "name": "String",
                                        "ofType": null
                                    },
                                    "defaultValue": null
                                },
                                {
                                    "name": "breed",
                                    "description": "",
                                    "type": {
                                        "kind": "SCALAR",
                                        "name": "Boolean",
                                        "ofType": null
                                    },
                                    "defaultValue": null
                                }
                            ],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "OBJECT",
                                    "name": "Dog",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "deleteDog",
                            "description": "",
                            "args": [
                                {
                                    "name": "id",
                                    "description": "",
                                    "type": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "SCALAR",
                                            "name": "ID",
                                            "ofType": null
                                        }
                                    },
                                    "defaultValue": null
                                }
                            ],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "Boolean",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "deleteDogByModal",
                            "description": "delete all dogs using their modal",
                            "args": [
                                {
                                    "name": "modal",
                                    "description": "",
                                    "type": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "SCALAR",
                                            "name": "String",
                                            "ofType": null
                                        }
                                    },
                                    "defaultValue": null
                                }
                            ],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "Boolean",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "updateDogName",
                            "description": "",
                            "args": [
                                {
                                    "name": "newName",
                                    "description": "",
                                    "type": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "SCALAR",
                                            "name": "String",
                                            "ofType": null
                                        }
                                    },
                                    "defaultValue": null
                                },
                                {
                                    "name": "id",
                                    "description": "",
                                    "type": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "SCALAR",
                                            "name": "ID",
                                            "ofType": null
                                        }
                                    },
                                    "defaultValue": null
                                }
                            ],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "OBJECT",
                                    "name": "Dog",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "updateDogBreed",
                            "description": "",
                            "args": [
                                {
                                    "name": "newBreed",
                                    "description": "",
                                    "type": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "SCALAR",
                                            "name": "Boolean",
                                            "ofType": null
                                        }
                                    },
                                    "defaultValue": null
                                },
                                {
                                    "name": "id",
                                    "description": "",
                                    "type": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "SCALAR",
                                            "name": "ID",
                                            "ofType": null
                                        }
                                    },
                                    "defaultValue": null
                                }
                            ],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "OBJECT",
                                    "name": "Dog",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        }
                    ],
                    "inputFields": null,
                    "interfaces": [],
                    "enumValues": null,
                    "possibleTypes": null
                },
                {
                    "kind": "SCALAR",
                    "name": "Boolean",
                    "description": "Built-in Boolean",
                    "fields": null,
                    "inputFields": null,
                    "interfaces": null,
                    "enumValues": null,
                    "possibleTypes": null
                },
                {
                    "kind": "OBJECT",
                    "name": "Dog",
                    "description": "a schema for the Object we have or database table",
                    "fields": [
                        {
                            "name": "id",
                            "description": "",
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "ID",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "name",
                            "description": "",
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "String",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "modal",
                            "description": "",
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "String",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "breed",
                            "description": "",
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "Boolean",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        }
                    ],
                    "inputFields": null,
                    "interfaces": [],
                    "enumValues": null,
                    "possibleTypes": null
                },
                {
                    "kind": "OBJECT",
                    "name": "__Schema",
                    "description": "A GraphQL Introspection defines the capabilities of a GraphQL server. It exposes all available types and directives on the server, the entry points for query, mutation, and subscription operations.",
                    "fields": [
                        {
                            "name": "types",
                            "description": "A list of all types supported by this server.",
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "LIST",
                                    "name": null,
                                    "ofType": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "OBJECT",
                                            "name": "__Type"
                                        }
                                    }
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "queryType",
                            "description": "The type that query operations will be rooted at.",
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "OBJECT",
                                    "name": "__Type",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "mutationType",
                            "description": "If this server supports mutation, the type that mutation operations will be rooted at.",
                            "args": [],
                            "type": {
                                "kind": "OBJECT",
                                "name": "__Type",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "directives",
                            "description": "'A list of all directives supported by this server.",
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "LIST",
                                    "name": null,
                                    "ofType": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "OBJECT",
                                            "name": "__Directive"
                                        }
                                    }
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "subscriptionType",
                            "description": "'If this server support subscription, the type that subscription operations will be rooted at.",
                            "args": [],
                            "type": {
                                "kind": "OBJECT",
                                "name": "__Type",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        }
                    ],
                    "inputFields": null,
                    "interfaces": [],
                    "enumValues": null,
                    "possibleTypes": null
                },
                {
                    "kind": "OBJECT",
                    "name": "__Type",
                    "description": null,
                    "fields": [
                        {
                            "name": "kind",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "ENUM",
                                    "name": "__TypeKind",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "name",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "SCALAR",
                                "name": "String",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "description",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "SCALAR",
                                "name": "String",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "fields",
                            "description": null,
                            "args": [
                                {
                                    "name": "includeDeprecated",
                                    "description": null,
                                    "type": {
                                        "kind": "SCALAR",
                                        "name": "Boolean",
                                        "ofType": null
                                    },
                                    "defaultValue": "false"
                                }
                            ],
                            "type": {
                                "kind": "LIST",
                                "name": null,
                                "ofType": {
                                    "kind": "NON_NULL",
                                    "name": null,
                                    "ofType": {
                                        "kind": "OBJECT",
                                        "name": "__Field",
                                        "ofType": null
                                    }
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "interfaces",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "LIST",
                                "name": null,
                                "ofType": {
                                    "kind": "NON_NULL",
                                    "name": null,
                                    "ofType": {
                                        "kind": "OBJECT",
                                        "name": "__Type",
                                        "ofType": null
                                    }
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "possibleTypes",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "LIST",
                                "name": null,
                                "ofType": {
                                    "kind": "NON_NULL",
                                    "name": null,
                                    "ofType": {
                                        "kind": "OBJECT",
                                        "name": "__Type",
                                        "ofType": null
                                    }
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "enumValues",
                            "description": null,
                            "args": [
                                {
                                    "name": "includeDeprecated",
                                    "description": null,
                                    "type": {
                                        "kind": "SCALAR",
                                        "name": "Boolean",
                                        "ofType": null
                                    },
                                    "defaultValue": "false"
                                }
                            ],
                            "type": {
                                "kind": "LIST",
                                "name": null,
                                "ofType": {
                                    "kind": "NON_NULL",
                                    "name": null,
                                    "ofType": {
                                        "kind": "OBJECT",
                                        "name": "__EnumValue",
                                        "ofType": null
                                    }
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "inputFields",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "LIST",
                                "name": null,
                                "ofType": {
                                    "kind": "NON_NULL",
                                    "name": null,
                                    "ofType": {
                                        "kind": "OBJECT",
                                        "name": "__InputValue",
                                        "ofType": null
                                    }
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "ofType",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "OBJECT",
                                "name": "__Type",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        }
                    ],
                    "inputFields": null,
                    "interfaces": [],
                    "enumValues": null,
                    "possibleTypes": null
                },
                {
                    "kind": "ENUM",
                    "name": "__TypeKind",
                    "description": "An enum describing what kind of type a given __Type is",
                    "fields": null,
                    "inputFields": null,
                    "interfaces": null,
                    "enumValues": [
                        {
                            "name": "SCALAR",
                            "description": "Indicates this type is a scalar.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "OBJECT",
                            "description": "Indicates this type is an object. `fields` and `interfaces` are valid fields.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "INTERFACE",
                            "description": "Indicates this type is an interface. `fields` and `possibleTypes` are valid fields.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "UNION",
                            "description": "Indicates this type is a union. `possibleTypes` is a valid field.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "ENUM",
                            "description": "Indicates this type is an enum. `enumValues` is a valid field.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "INPUT_OBJECT",
                            "description": "Indicates this type is an input object. `inputFields` is a valid field.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "LIST",
                            "description": "Indicates this type is a list. `ofType` is a valid field.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "NON_NULL",
                            "description": "Indicates this type is a non-null. `ofType` is a valid field.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        }
                    ],
                    "possibleTypes": null
                },
                {
                    "kind": "OBJECT",
                    "name": "__Field",
                    "description": null,
                    "fields": [
                        {
                            "name": "name",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "String",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "description",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "SCALAR",
                                "name": "String",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "args",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "LIST",
                                    "name": null,
                                    "ofType": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "OBJECT",
                                            "name": "__InputValue"
                                        }
                                    }
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "type",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "OBJECT",
                                    "name": "__Type",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "isDeprecated",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "Boolean",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "deprecationReason",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "SCALAR",
                                "name": "String",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        }
                    ],
                    "inputFields": null,
                    "interfaces": [],
                    "enumValues": null,
                    "possibleTypes": null
                },
                {
                    "kind": "OBJECT",
                    "name": "__InputValue",
                    "description": null,
                    "fields": [
                        {
                            "name": "name",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "String",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "description",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "SCALAR",
                                "name": "String",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "type",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "OBJECT",
                                    "name": "__Type",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "defaultValue",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "SCALAR",
                                "name": "String",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        }
                    ],
                    "inputFields": null,
                    "interfaces": [],
                    "enumValues": null,
                    "possibleTypes": null
                },
                {
                    "kind": "OBJECT",
                    "name": "__EnumValue",
                    "description": null,
                    "fields": [
                        {
                            "name": "name",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "String",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "description",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "SCALAR",
                                "name": "String",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "isDeprecated",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "Boolean",
                                    "ofType": null
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "deprecationReason",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "SCALAR",
                                "name": "String",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        }
                    ],
                    "inputFields": null,
                    "interfaces": [],
                    "enumValues": null,
                    "possibleTypes": null
                },
                {
                    "kind": "OBJECT",
                    "name": "__Directive",
                    "description": null,
                    "fields": [
                        {
                            "name": "name",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "SCALAR",
                                "name": "String",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "description",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "SCALAR",
                                "name": "String",
                                "ofType": null
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "locations",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "LIST",
                                "name": null,
                                "ofType": {
                                    "kind": "NON_NULL",
                                    "name": null,
                                    "ofType": {
                                        "kind": "ENUM",
                                        "name": "__DirectiveLocation",
                                        "ofType": null
                                    }
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "args",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "LIST",
                                    "name": null,
                                    "ofType": {
                                        "kind": "NON_NULL",
                                        "name": null,
                                        "ofType": {
                                            "kind": "OBJECT",
                                            "name": "__InputValue"
                                        }
                                    }
                                }
                            },
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "onOperation",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "SCALAR",
                                "name": "Boolean",
                                "ofType": null
                            },
                            "isDeprecated": true,
                            "deprecationReason": "Use `locations`."
                        },
                        {
                            "name": "onFragment",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "SCALAR",
                                "name": "Boolean",
                                "ofType": null
                            },
                            "isDeprecated": true,
                            "deprecationReason": "Use `locations`."
                        },
                        {
                            "name": "onField",
                            "description": null,
                            "args": [],
                            "type": {
                                "kind": "SCALAR",
                                "name": "Boolean",
                                "ofType": null
                            },
                            "isDeprecated": true,
                            "deprecationReason": "Use `locations`."
                        }
                    ],
                    "inputFields": null,
                    "interfaces": [],
                    "enumValues": null,
                    "possibleTypes": null
                },
                {
                    "kind": "ENUM",
                    "name": "__DirectiveLocation",
                    "description": "An enum describing valid locations where a directive can be placed",
                    "fields": null,
                    "inputFields": null,
                    "interfaces": null,
                    "enumValues": [
                        {
                            "name": "QUERY",
                            "description": "Indicates the directive is valid on queries.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "MUTATION",
                            "description": "Indicates the directive is valid on mutations.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "FIELD",
                            "description": "Indicates the directive is valid on fields.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "FRAGMENT_DEFINITION",
                            "description": "Indicates the directive is valid on fragment definitions.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "FRAGMENT_SPREAD",
                            "description": "Indicates the directive is valid on fragment spreads.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "INLINE_FRAGMENT",
                            "description": "Indicates the directive is valid on inline fragments.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "SCHEMA",
                            "description": "Indicates the directive is valid on a schema SDL definition.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "SCALAR",
                            "description": "Indicates the directive is valid on a scalar SDL definition.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "OBJECT",
                            "description": "Indicates the directive is valid on an object SDL definition.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "FIELD_DEFINITION",
                            "description": "Indicates the directive is valid on a field SDL definition.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "ARGUMENT_DEFINITION",
                            "description": "Indicates the directive is valid on a field argument SDL definition.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "INTERFACE",
                            "description": "Indicates the directive is valid on an interface SDL definition.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "UNION",
                            "description": "Indicates the directive is valid on an union SDL definition.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "ENUM",
                            "description": "Indicates the directive is valid on an enum SDL definition.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "ENUM_VALUE",
                            "description": "Indicates the directive is valid on an enum value SDL definition.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "INPUT_OBJECT",
                            "description": "Indicates the directive is valid on an input object SDL definition.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        },
                        {
                            "name": "INPUT_FIELD_DEFINITION",
                            "description": "Indicates the directive is valid on an input object field SDL definition.",
                            "isDeprecated": false,
                            "deprecationReason": null
                        }
                    ],
                    "possibleTypes": null
                }
            ],
            "directives": [
                {
                    "name": "include",
                    "description": "Directs the executor to include this field or fragment only when the `if` argument is true",
                    "locations": [
                        "FIELD",
                        "FRAGMENT_SPREAD",
                        "INLINE_FRAGMENT"
                    ],
                    "args": [
                        {
                            "name": "if",
                            "description": "Included when true.",
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "Boolean",
                                    "ofType": null
                                }
                            },
                            "defaultValue": null
                        }
                    ]
                },
                {
                    "name": "skip",
                    "description": "Directs the executor to skip this field or fragment when the `if`'argument is true.",
                    "locations": [
                        "FIELD",
                        "FRAGMENT_SPREAD",
                        "INLINE_FRAGMENT"
                    ],
                    "args": [
                        {
                            "name": "if",
                            "description": "Skipped when true.",
                            "type": {
                                "kind": "NON_NULL",
                                "name": null,
                                "ofType": {
                                    "kind": "SCALAR",
                                    "name": "Boolean",
                                    "ofType": null
                                }
                            },
                            "defaultValue": null
                        }
                    ]
                },
                {
                    "name": "defer",
                    "description": "This directive allows results to be deferred during execution",
                    "locations": [
                        "FIELD"
                    ],
                    "args": []
                }
            ]
        }
    }
}
```
