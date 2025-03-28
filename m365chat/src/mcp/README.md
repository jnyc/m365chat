# M365Chat - MCP Server for Microsoft Graph

M365Chat is an MCP server for querying and managing your Microsoft 365 tenant using the Microsoft Graph API. It acts as a bridge between the Microsoft Graph API and any compatible MCP client, allowing you to interact with your Microsoft 365 tenant using natural language queries.

## Sample queries

Here are some examples of queries you can use with Lokka.

- `Create a new security group called 'Sales and HR' with a dynamic rule based on the department attribute.`
- `Find all the conditional access policies that haven't excluded the emergency access account`
- `Show me all the device configuration policies assigned to the 'Call center' group`

## What is M365Chat?

Lokka is designed to be used with any compatible MCP client, such as Claude Desktop, Cursor, Goose, or any other AI model and client that support the Model Context Protocol. It provides a simple and intuitive way to manage your Microsoft 365 tenant using natural language queries.

## MCP Client Configuration

```json
{
  "mcpServers": {
    "Lokka-Microsoft-Graph": {
      "command": "npx",
      "args": ["-y", "@suarez999/m365chat"],
      "env": {
        "TENANT_ID": "<tenant-id>",
        "CLIENT_ID": "<client-id>",
        "CLIENT_SECRET": "<client-secret>"
      }
    }
  }
}
```

## Get started

See the docs for more information on how to install and configure m365chat based on Lokka.

- [Introduction](https://lokka.dev/docs/intro)
- [Install guide](https://lokka.dev/docs/installation)
- [Developer guide](https://lokka.dev/docs/developer-guide)
