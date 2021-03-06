---
enableInlineShortcodes: true
bookToC: false
---
Voyager is an interactive GraphQL API explorer. It allows you to view all the data in our API. Click and drag to move around the explorer. Click on a field to view its properties. Scoll to adjust zoom.

{{< rawhtml >}}
    <div id="voyager">Loading...</div>

<script>
  
  // Render <Voyager />
    GraphQLVoyager.init(document.getElementById('voyager'), {
      hideDocs: true,
      hideSettings: false,
      displayOptions: {
        sortByAlphabet: true,
      },
      introspection: {
  "data": {
    "__schema": {
      "directives": [
        {
          "args": [
            {
              "defaultValue": null,
              "description": "Included when true.",
              "name": "if",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "Boolean",
                  "ofType": null
                }
              }
            }
          ],
          "description": "Directs the executor to include this field or fragment only when the `if` argument is true.",
          "locations": [
            "FIELD",
            "FRAGMENT_SPREAD",
            "INLINE_FRAGMENT"
          ],
          "name": "include"
        },
        {
          "args": [
            {
              "defaultValue": null,
              "description": "Skipped when true.",
              "name": "if",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "Boolean",
                  "ofType": null
                }
              }
            }
          ],
          "description": "Directs the executor to skip this field or fragment when the `if` argument is true.",
          "locations": [
            "FIELD",
            "FRAGMENT_SPREAD",
            "INLINE_FRAGMENT"
          ],
          "name": "skip"
        }
      ],
      "mutationType": {
        "name": "RootMutationType"
      },
      "queryType": {
        "name": "RootQueryType"
      },
      "types": [
        {
          "description": "A moderation event that happened",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "action",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "channel",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "Channel",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "insertedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "moderator",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "User",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "updatedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "user",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "User",
                  "ofType": null
                }
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "ChannelModerationLog",
          "possibleTypes": null
        },
        {
          "description": "A channel moderator",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "canBan",
              "type": {
                "kind": "SCALAR",
                "name": "Boolean",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "canLongTimeout",
              "type": {
                "kind": "SCALAR",
                "name": "Boolean",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "canShortTimeout",
              "type": {
                "kind": "SCALAR",
                "name": "Boolean",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "canUnTimeout",
              "type": {
                "kind": "SCALAR",
                "name": "Boolean",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "canUnban",
              "type": {
                "kind": "SCALAR",
                "name": "Boolean",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "channel",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "Channel",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "insertedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "updatedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "user",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "User",
                  "ofType": null
                }
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "ChannelModerator",
          "possibleTypes": null
        },
        {
          "description": "Represents scalars, interfaces, object types, unions, enums in the system",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "description",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": "false",
                  "description": null,
                  "name": "includeDeprecated",
                  "type": {
                    "kind": "SCALAR",
                    "name": "Boolean",
                    "ofType": null
                  }
                }
              ],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "enumValues",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "__EnumValue",
                  "ofType": null
                }
              }
            },
            {
              "args": [
                {
                  "defaultValue": "false",
                  "description": null,
                  "name": "includeDeprecated",
                  "type": {
                    "kind": "SCALAR",
                    "name": "Boolean",
                    "ofType": null
                  }
                }
              ],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "fields",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "__Field",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "inputFields",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "__InputValue",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "interfaces",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "__Type",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "kind",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "name",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "ofType",
              "type": {
                "kind": "OBJECT",
                "name": "__Type",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "possibleTypes",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "__Type",
                  "ofType": null
                }
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "__Type",
          "possibleTypes": null
        },
        {
          "description": "The `Boolean` scalar type represents `true` or `false`.",
          "enumValues": null,
          "fields": null,
          "inputFields": null,
          "interfaces": null,
          "kind": "SCALAR",
          "name": "Boolean",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": null,
          "fields": [
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "id",
                  "type": {
                    "kind": "SCALAR",
                    "name": "ID",
                    "ofType": null
                  }
                }
              ],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "channel",
              "type": {
                "kind": "OBJECT",
                "name": "Channel",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "channelId",
                  "type": {
                    "kind": "SCALAR",
                    "name": "ID",
                    "ofType": null
                  }
                }
              ],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "chatMessage",
              "type": {
                "kind": "OBJECT",
                "name": "ChatMessage",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "streamerId",
                  "type": {
                    "kind": "SCALAR",
                    "name": "ID",
                    "ofType": null
                  }
                }
              ],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "followers",
              "type": {
                "kind": "OBJECT",
                "name": "Follower",
                "ofType": null
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "RootSubscriptionType",
          "possibleTypes": null
        },
        {
          "description": "A single instance of stream metadata.",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "audioCodec",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "id",
              "type": {
                "kind": "SCALAR",
                "name": "ID",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "ingestServer",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "ingestViewers",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "insertedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "lostPackets",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "nackPackets",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "recvPackets",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "sourceBitrate",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "sourcePing",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "stream",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "Stream",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "streamTimeSeconds",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "updatedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "vendorName",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "vendorVersion",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "videoCodec",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "videoHeight",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "videoWidth",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "StreamMetadata",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": null,
          "fields": null,
          "inputFields": [
            {
              "defaultValue": null,
              "description": null,
              "name": "audioCodec",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "defaultValue": null,
              "description": null,
              "name": "ingestServer",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "defaultValue": null,
              "description": null,
              "name": "ingestViewers",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "defaultValue": null,
              "description": null,
              "name": "lostPackets",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "defaultValue": null,
              "description": null,
              "name": "nackPackets",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "defaultValue": null,
              "description": null,
              "name": "recvPackets",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "defaultValue": null,
              "description": null,
              "name": "sourceBitrate",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "defaultValue": null,
              "description": null,
              "name": "sourcePing",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "defaultValue": null,
              "description": null,
              "name": "streamTimeSeconds",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "defaultValue": null,
              "description": null,
              "name": "vendorName",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "defaultValue": null,
              "description": null,
              "name": "vendorVersion",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "defaultValue": null,
              "description": null,
              "name": "videoCodec",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "defaultValue": null,
              "description": null,
              "name": "videoHeight",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "defaultValue": null,
              "description": null,
              "name": "videoWidth",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            }
          ],
          "interfaces": null,
          "kind": "INPUT_OBJECT",
          "name": "StreamMetadataInput",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": null,
          "fields": null,
          "inputFields": [
            {
              "defaultValue": null,
              "description": null,
              "name": "message",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            }
          ],
          "interfaces": null,
          "kind": "INPUT_OBJECT",
          "name": "ChatMessageInput",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "text",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "type",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "url",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            }
          ],
          "inputFields": null,
          "interfaces": [
            {
              "kind": "INTERFACE",
              "name": "ChatMessageToken",
              "ofType": null
            }
          ],
          "kind": "OBJECT",
          "name": "UrlToken",
          "possibleTypes": null
        },
        {
          "description": "Represents a directive",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "args",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "__InputValue",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "description",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "locations",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "ENUM",
                  "name": "__DirectiveLocation",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "name",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": "Check `locations` field for enum value FIELD",
              "description": null,
              "isDeprecated": true,
              "name": "onField",
              "type": {
                "kind": "SCALAR",
                "name": "Boolean",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": "Check `locations` field for enum value FRAGMENT_SPREAD",
              "description": null,
              "isDeprecated": true,
              "name": "onFragment",
              "type": {
                "kind": "SCALAR",
                "name": "Boolean",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": "Check `locations` field for enum value OPERATION",
              "description": null,
              "isDeprecated": true,
              "name": "onOperation",
              "type": {
                "kind": "SCALAR",
                "name": "Boolean",
                "ofType": null
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "__Directive",
          "possibleTypes": null
        },
        {
          "description": "A subscription is an exchange of money for support.",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "endedAt",
              "type": {
                "kind": "SCALAR",
                "name": "DateTime",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "id",
              "type": {
                "kind": "SCALAR",
                "name": "ID",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "insertedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "isActive",
              "type": {
                "kind": "SCALAR",
                "name": "Boolean",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "price",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "productName",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "startedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "DateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "streamer",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "User",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "updatedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "user",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "User",
                  "ofType": null
                }
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "Sub",
          "possibleTypes": null
        },
        {
          "description": "A channel is a user's actual container for live streaming.",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "bans",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "ChannelBan",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "category",
              "type": {
                "kind": "OBJECT",
                "name": "Category",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "chatMessages",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "ChatMessage",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "chatRulesHtml",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "chatRulesMd",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "hmacKey",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "id",
              "type": {
                "kind": "SCALAR",
                "name": "ID",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "inaccessible",
              "type": {
                "kind": "SCALAR",
                "name": "Boolean",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "insertedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "The language a user can expect in the stream.",
              "isDeprecated": false,
              "name": "language",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "moderationLogs",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "ChannelModerationLog",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "moderators",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "ChannelModerator",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "status",
              "type": {
                "kind": "ENUM",
                "name": "ChannelStatus",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "stream",
              "type": {
                "kind": "OBJECT",
                "name": "Stream",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "streamKey",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "streamer",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "User",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "tags",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "Tag",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "thumbnail",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "The title of the current stream, live or offline.",
              "isDeprecated": false,
              "name": "title",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "updatedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": "Please use the streamer field",
              "description": null,
              "isDeprecated": true,
              "name": "user",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "User",
                  "ofType": null
                }
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "Channel",
          "possibleTypes": null
        },
        {
          "description": "A stream is a single live stream in, either current or historical.",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "avgChatters",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "avgViewers",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "category",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "Category",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "channel",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "Channel",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "countChatters",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "countViewers",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "endedAt",
              "type": {
                "kind": "SCALAR",
                "name": "NaiveDateTime",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "id",
              "type": {
                "kind": "SCALAR",
                "name": "ID",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "insertedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "metadata",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "StreamMetadata",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "newSubscribers",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "peakChatters",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "peakViewers",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "resubSubscribers",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "startedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "thumbnail",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "The title of the stream.",
              "isDeprecated": false,
              "name": "title",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "updatedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "Stream",
          "possibleTypes": null
        },
        {
          "description": "A user of Glimesh, can be a streamer, a viewer or both!",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "avatar",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "avatarUrl",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "confirmedAt",
              "type": {
                "kind": "SCALAR",
                "name": "NaiveDateTime",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Exactly the same as the username, but with casing the user prefers",
              "isDeprecated": false,
              "name": "displayname",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "id",
              "type": {
                "kind": "SCALAR",
                "name": "ID",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "HTML version of the user's profile, should be safe for rendering directly",
              "isDeprecated": false,
              "name": "profileContentHtml",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Markdown version of the user's profile",
              "isDeprecated": false,
              "name": "profileContentMd",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Qualified URL for the user's Discord server",
              "isDeprecated": false,
              "name": "socialDiscord",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Qualified URL for the user's Guilded server",
              "isDeprecated": false,
              "name": "socialGuilded",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Qualified URL for the user's Instagram account",
              "isDeprecated": false,
              "name": "socialInstagram",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": "Use the socials field instead",
              "description": "Qualified URL for the user's Twitter account",
              "isDeprecated": true,
              "name": "socialTwitter",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Qualified URL for the user's YouTube account",
              "isDeprecated": false,
              "name": "socialYoutube",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "A list of linked social accounts for the user",
              "isDeprecated": false,
              "name": "socials",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "UserSocial",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Lowercase user identifier",
              "isDeprecated": false,
              "name": "username",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "YouTube Intro URL for the user's profile",
              "isDeprecated": false,
              "name": "youtubeIntroUrl",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "User",
          "possibleTypes": null
        },
        {
          "description": "The `String` scalar type represents textual data, represented as UTF-8\ncharacter sequences. The String type is most often used by GraphQL to\nrepresent free-form human-readable text.",
          "enumValues": null,
          "fields": null,
          "inputFields": null,
          "interfaces": null,
          "kind": "SCALAR",
          "name": "String",
          "possibleTypes": null
        },
        {
          "description": "Tags are user created labels that are either global or category specific.",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "category",
              "type": {
                "kind": "OBJECT",
                "name": "Category",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "The number of streams started with this tag",
              "isDeprecated": false,
              "name": "countUsage",
              "type": {
                "kind": "SCALAR",
                "name": "Int",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "id",
              "type": {
                "kind": "SCALAR",
                "name": "ID",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "insertedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Name of the tag",
              "isDeprecated": false,
              "name": "name",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "URL friendly name of the tag",
              "isDeprecated": false,
              "name": "slug",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "updatedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "Tag",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": null,
          "fields": [
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "channelId",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "ID",
                      "ofType": null
                    }
                  }
                },
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "userId",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "ID",
                      "ofType": null
                    }
                  }
                }
              ],
              "deprecationReason": null,
              "description": "Ban a user from a chat channel.",
              "isDeprecated": false,
              "name": "banUser",
              "type": {
                "kind": "OBJECT",
                "name": "ChannelModerationLog",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "channelId",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "ID",
                      "ofType": null
                    }
                  }
                },
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "message",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "INPUT_OBJECT",
                      "name": "ChatMessageInput",
                      "ofType": null
                    }
                  }
                }
              ],
              "deprecationReason": null,
              "description": "Create a chat message",
              "isDeprecated": false,
              "name": "createChatMessage",
              "type": {
                "kind": "OBJECT",
                "name": "ChatMessage",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "streamId",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "ID",
                      "ofType": null
                    }
                  }
                }
              ],
              "deprecationReason": null,
              "description": "End a stream",
              "isDeprecated": false,
              "name": "endStream",
              "type": {
                "kind": "OBJECT",
                "name": "Stream",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "metadata",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "INPUT_OBJECT",
                      "name": "StreamMetadataInput",
                      "ofType": null
                    }
                  }
                },
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "streamId",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "ID",
                      "ofType": null
                    }
                  }
                }
              ],
              "deprecationReason": null,
              "description": "Update a stream's metadata",
              "isDeprecated": false,
              "name": "logStreamMetadata",
              "type": {
                "kind": "OBJECT",
                "name": "Stream",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "channelId",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "ID",
                      "ofType": null
                    }
                  }
                },
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "userId",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "ID",
                      "ofType": null
                    }
                  }
                }
              ],
              "deprecationReason": null,
              "description": "Long timeout (15 minutes) a user from a chat channel.",
              "isDeprecated": false,
              "name": "longTimeoutUser",
              "type": {
                "kind": "OBJECT",
                "name": "ChannelModerationLog",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "channelId",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "ID",
                      "ofType": null
                    }
                  }
                },
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "userId",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "ID",
                      "ofType": null
                    }
                  }
                }
              ],
              "deprecationReason": null,
              "description": "Short timeout (5 minutes) a user from a chat channel.",
              "isDeprecated": false,
              "name": "shortTimeoutUser",
              "type": {
                "kind": "OBJECT",
                "name": "ChannelModerationLog",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "channelId",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "ID",
                      "ofType": null
                    }
                  }
                }
              ],
              "deprecationReason": null,
              "description": "Start a stream",
              "isDeprecated": false,
              "name": "startStream",
              "type": {
                "kind": "OBJECT",
                "name": "Stream",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "channelId",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "ID",
                      "ofType": null
                    }
                  }
                },
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "userId",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "ID",
                      "ofType": null
                    }
                  }
                }
              ],
              "deprecationReason": null,
              "description": "Unban a user from a chat channel.",
              "isDeprecated": false,
              "name": "unbanUser",
              "type": {
                "kind": "OBJECT",
                "name": "ChannelModerationLog",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "streamId",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "ID",
                      "ofType": null
                    }
                  }
                },
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "thumbnail",
                  "type": {
                    "kind": "NON_NULL",
                    "name": null,
                    "ofType": {
                      "kind": "SCALAR",
                      "name": "Upload",
                      "ofType": null
                    }
                  }
                }
              ],
              "deprecationReason": null,
              "description": "Update a stream's thumbnail",
              "isDeprecated": false,
              "name": "uploadStreamThumbnail",
              "type": {
                "kind": "OBJECT",
                "name": "Stream",
                "ofType": null
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "RootMutationType",
          "possibleTypes": null
        },
        {
          "description": "A linked social account for a Glimesh user.",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "id",
              "type": {
                "kind": "SCALAR",
                "name": "ID",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Platform unique identifier, usually a ID, made into a string",
              "isDeprecated": false,
              "name": "identifier",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "insertedAt",
              "type": {
                "kind": "SCALAR",
                "name": "NaiveDateTime",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Platform that is linked, eg: twitter",
              "isDeprecated": false,
              "name": "platform",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "updatedAt",
              "type": {
                "kind": "SCALAR",
                "name": "NaiveDateTime",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Username for the user on the linked platform",
              "isDeprecated": false,
              "name": "username",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "UserSocial",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "text",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "type",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            }
          ],
          "inputFields": null,
          "interfaces": null,
          "kind": "INTERFACE",
          "name": "ChatMessageToken",
          "possibleTypes": [
            {
              "kind": "OBJECT",
              "name": "EmoteToken",
              "ofType": null
            },
            {
              "kind": "OBJECT",
              "name": "TextToken",
              "ofType": null
            },
            {
              "kind": "OBJECT",
              "name": "UrlToken",
              "ofType": null
            }
          ]
        },
        {
          "description": "The `Naive DateTime` scalar type represents a naive date and time without\ntimezone. The DateTime appears in a JSON response as an ISO8601 formatted\nstring.",
          "enumValues": null,
          "fields": null,
          "inputFields": null,
          "interfaces": null,
          "kind": "SCALAR",
          "name": "NaiveDateTime",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "deprecationReason",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "description",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "isDeprecated",
              "type": {
                "kind": "SCALAR",
                "name": "Boolean",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "name",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "__EnumValue",
          "possibleTypes": null
        },
        {
          "description": "The `DateTime` scalar type represents a date and time in the UTC\ntimezone. The DateTime appears in a JSON response as an ISO8601 formatted\nstring, including UTC timezone (\"Z\"). The parsed date and time string will\nbe converted to UTC if there is an offset.",
          "enumValues": null,
          "fields": null,
          "inputFields": null,
          "interfaces": null,
          "kind": "SCALAR",
          "name": "DateTime",
          "possibleTypes": null
        },
        {
          "description": "A follower is a user who subscribes to notifications for a particular user's channel.",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "hasLiveNotifications",
              "type": {
                "kind": "SCALAR",
                "name": "Boolean",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "id",
              "type": {
                "kind": "SCALAR",
                "name": "ID",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "insertedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "streamer",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "User",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "updatedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "user",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "User",
                  "ofType": null
                }
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "Follower",
          "possibleTypes": null
        },
        {
          "description": "Represents an uploaded file.\n",
          "enumValues": null,
          "fields": null,
          "inputFields": null,
          "interfaces": null,
          "kind": "SCALAR",
          "name": "Upload",
          "possibleTypes": null
        },
        {
          "description": "Categories are the containers for live streaming content.",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "id",
              "type": {
                "kind": "SCALAR",
                "name": "ID",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Name of the category",
              "isDeprecated": false,
              "name": "name",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": "All categories are now parents and the children are tags.",
              "description": null,
              "isDeprecated": true,
              "name": "parent",
              "type": {
                "kind": "OBJECT",
                "name": "Category",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Slug of the category",
              "isDeprecated": false,
              "name": "slug",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": "Tag name is now just name",
              "description": null,
              "isDeprecated": true,
              "name": "tagName",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "tags",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "Tag",
                  "ofType": null
                }
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "Category",
          "possibleTypes": null
        },
        {
          "description": "The `ID` scalar type represents a unique identifier, often used to\nrefetch an object or as key for a cache. The ID type appears in a JSON\nresponse as a String; however, it is not intended to be human-readable.\nWhen expected as an input type, any string (such as `\"4\"`) or integer\n(such as `4`) input value will be accepted as an ID.",
          "enumValues": null,
          "fields": null,
          "inputFields": null,
          "interfaces": null,
          "kind": "SCALAR",
          "name": "ID",
          "possibleTypes": null
        },
        {
          "description": "Represents a schema",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "directives",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "__Directive",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "mutationType",
              "type": {
                "kind": "OBJECT",
                "name": "__Type",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "queryType",
              "type": {
                "kind": "OBJECT",
                "name": "__Type",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "subscriptionType",
              "type": {
                "kind": "OBJECT",
                "name": "__Type",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "types",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "__Type",
                  "ofType": null
                }
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "__Schema",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": [
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "ARGUMENT_DEFINITION"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "ENUM"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "ENUM_VALUE"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "FIELD"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "FIELD_DEFINITION"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "FRAGMENT_DEFINITION"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "FRAGMENT_SPREAD"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "INLINE_FRAGMENT"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "INPUT_FIELD_DEFINITION"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "INPUT_OBJECT"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "INTERFACE"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "MUTATION"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "OBJECT"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "QUERY"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "SCALAR"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "SCHEMA"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "SUBSCRIPTION"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "UNION"
            }
          ],
          "fields": null,
          "inputFields": null,
          "interfaces": null,
          "kind": "ENUM",
          "name": "__DirectiveLocation",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": [
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "LIVE"
            },
            {
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "OFFLINE"
            }
          ],
          "fields": null,
          "inputFields": null,
          "interfaces": null,
          "kind": "ENUM",
          "name": "ChannelStatus",
          "possibleTypes": null
        },
        {
          "description": "The `Int` scalar type represents non-fractional signed whole numeric values.\nInt can represent values between `-(2^53 - 1)` and `2^53 - 1` since it is\nrepresented in JSON as double-precision floating point numbers specified\nby [IEEE 754](http://en.wikipedia.org/wiki/IEEE_floating_point).",
          "enumValues": null,
          "fields": null,
          "inputFields": null,
          "interfaces": null,
          "kind": "SCALAR",
          "name": "Int",
          "possibleTypes": null
        },
        {
          "description": "A channel timeout or ban",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "channel",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "Channel",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "expiresAt",
              "type": {
                "kind": "SCALAR",
                "name": "NaiveDateTime",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "insertedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "reason",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "updatedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "user",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "User",
                  "ofType": null
                }
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "ChannelBan",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "args",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "__InputValue",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "deprecationReason",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "description",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "isDeprecated",
              "type": {
                "kind": "SCALAR",
                "name": "Boolean",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "name",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "type",
              "type": {
                "kind": "OBJECT",
                "name": "__Type",
                "ofType": null
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "__Field",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "defaultValue",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "description",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "name",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "type",
              "type": {
                "kind": "OBJECT",
                "name": "__Type",
                "ofType": null
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "__InputValue",
          "possibleTypes": null
        },
        {
          "description": "A chat message sent to a channel by a user.",
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "channel",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "Channel",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "id",
              "type": {
                "kind": "SCALAR",
                "name": "ID",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "insertedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "The chat message.",
              "isDeprecated": false,
              "name": "message",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "tokens",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "INTERFACE",
                  "name": "ChatMessageToken",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "updatedAt",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "SCALAR",
                  "name": "NaiveDateTime",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "user",
              "type": {
                "kind": "NON_NULL",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "User",
                  "ofType": null
                }
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "ChatMessage",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "src",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "text",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "type",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "url",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            }
          ],
          "inputFields": null,
          "interfaces": [
            {
              "kind": "INTERFACE",
              "name": "ChatMessageToken",
              "ofType": null
            }
          ],
          "kind": "OBJECT",
          "name": "EmoteToken",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": "List all categories",
              "isDeprecated": false,
              "name": "categories",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "Category",
                  "ofType": null
                }
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "slug",
                  "type": {
                    "kind": "SCALAR",
                    "name": "String",
                    "ofType": null
                  }
                }
              ],
              "deprecationReason": null,
              "description": "Query individual category",
              "isDeprecated": false,
              "name": "category",
              "type": {
                "kind": "OBJECT",
                "name": "Category",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "hmacKey",
                  "type": {
                    "kind": "SCALAR",
                    "name": "String",
                    "ofType": null
                  }
                },
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "id",
                  "type": {
                    "kind": "SCALAR",
                    "name": "ID",
                    "ofType": null
                  }
                },
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "username",
                  "type": {
                    "kind": "SCALAR",
                    "name": "String",
                    "ofType": null
                  }
                }
              ],
              "deprecationReason": null,
              "description": "Query individual channel",
              "isDeprecated": false,
              "name": "channel",
              "type": {
                "kind": "OBJECT",
                "name": "Channel",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "categorySlug",
                  "type": {
                    "kind": "SCALAR",
                    "name": "String",
                    "ofType": null
                  }
                },
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "status",
                  "type": {
                    "kind": "ENUM",
                    "name": "ChannelStatus",
                    "ofType": null
                  }
                }
              ],
              "deprecationReason": null,
              "description": "List all channels",
              "isDeprecated": false,
              "name": "channels",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "Channel",
                  "ofType": null
                }
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "streamerUsername",
                  "type": {
                    "kind": "SCALAR",
                    "name": "String",
                    "ofType": null
                  }
                },
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "userUsername",
                  "type": {
                    "kind": "SCALAR",
                    "name": "String",
                    "ofType": null
                  }
                }
              ],
              "deprecationReason": null,
              "description": "List all follows or followers",
              "isDeprecated": false,
              "name": "followers",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "Follower",
                  "ofType": null
                }
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "Get yourself",
              "isDeprecated": false,
              "name": "myself",
              "type": {
                "kind": "OBJECT",
                "name": "User",
                "ofType": null
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "streamerUsername",
                  "type": {
                    "kind": "SCALAR",
                    "name": "String",
                    "ofType": null
                  }
                },
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "userUsername",
                  "type": {
                    "kind": "SCALAR",
                    "name": "String",
                    "ofType": null
                  }
                }
              ],
              "deprecationReason": null,
              "description": "List all subscribers or subscribees",
              "isDeprecated": false,
              "name": "subscriptions",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "Sub",
                  "ofType": null
                }
              }
            },
            {
              "args": [
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "id",
                  "type": {
                    "kind": "SCALAR",
                    "name": "Int",
                    "ofType": null
                  }
                },
                {
                  "defaultValue": null,
                  "description": null,
                  "name": "username",
                  "type": {
                    "kind": "SCALAR",
                    "name": "String",
                    "ofType": null
                  }
                }
              ],
              "deprecationReason": null,
              "description": "Query individual user",
              "isDeprecated": false,
              "name": "user",
              "type": {
                "kind": "OBJECT",
                "name": "User",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": "List all users",
              "isDeprecated": false,
              "name": "users",
              "type": {
                "kind": "LIST",
                "name": null,
                "ofType": {
                  "kind": "OBJECT",
                  "name": "User",
                  "ofType": null
                }
              }
            }
          ],
          "inputFields": null,
          "interfaces": [],
          "kind": "OBJECT",
          "name": "RootQueryType",
          "possibleTypes": null
        },
        {
          "description": null,
          "enumValues": null,
          "fields": [
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "text",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            },
            {
              "args": [],
              "deprecationReason": null,
              "description": null,
              "isDeprecated": false,
              "name": "type",
              "type": {
                "kind": "SCALAR",
                "name": "String",
                "ofType": null
              }
            }
          ],
          "inputFields": null,
          "interfaces": [
            {
              "kind": "INTERFACE",
              "name": "ChatMessageToken",
              "ofType": null
            }
          ],
          "kind": "OBJECT",
          "name": "TextToken",
          "possibleTypes": null
        }
      ]
    }
  }
},
    });
    // Sets the settings to a dark color
 //   var menuThingy = document.getElementsByClassName("menu-content");
   // menuThingy[0].style.backgroundColor = "#0e1726";
    // Sets the navbar to the left. Doesn't do much, just gives appearance of more space.
  //  var navBar = document.getElementsByTagName("nav");
   // navBar[0].style.left = 0;
    // dark colors
   // var voyagerPanel = document.getElementsByClassName("doc-navigation");
    //voyagerPanel[0].style.background = "#0e1726"
   // var voyagerPanel = document.getElementsByClassName("scroll-area");
   // voyagerPanel[0].style.background = "#0e1726";
   // var voyagerPanel = document.getElementsByClassName("contents");
   // voyagerPanel[0].style.background = "#0e1726"
   // var voyagerPanel = document.getElementsByClassName("doc-panel");
   // voyagerPanel[0].style.position = "absolute"
    // Makes the panel draggable, hopefully users will move it to a better position. 
   // dragElement(voyagerPanel[0]);

function dragElement(elmnt) {
  var pos1 = 0, pos2 = 0, pos3 = 0, pos4 = 0;
    elmnt.onmousedown = dragMouseDown;


  function dragMouseDown(e) {
    e = e || window.event;
    e.preventDefault();
    // get the mouse cursor position at startup:
    pos3 = e.clientX;
    pos4 = e.clientY;
    document.onmouseup = closeDragElement;
    // call a function whenever the cursor moves:
    document.onmousemove = elementDrag;
  }

  function elementDrag(e) {
    e = e || window.event;
    e.preventDefault();
    // calculate the new cursor position:
    pos1 = pos3 - e.clientX;
    pos2 = pos4 - e.clientY;
    pos3 = e.clientX;
    pos4 = e.clientY;
    // set the element's new position:
    elmnt.style.top = (elmnt.offsetTop - pos2) + "px";
    elmnt.style.left = (elmnt.offsetLeft - pos1) + "px";
  }

  function closeDragElement() {
    // stop moving when mouse button is released:
    document.onmouseup = null;
    document.onmousemove = null;
  }
}

  </script>
{{< /rawhtml >}}
