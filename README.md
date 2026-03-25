# Nitro MCP Publish

A GitHub Action that publishes MCP feature collections to the Nitro registry.

## Usage

```yaml
- uses: ChilliCream/nitro-mcp-publish@v16
  with:
    tag: <tag>
    stage: <stage>
    mcp-feature-collection-id: <mcp-feature-collection-id>
    api-key: <api-key>
    # Optional
    force: false
    wait-for-approval: false
    cloud-url: <cloud-url>
    job-id: <job-id>
```

## Inputs

| Name                        | Required | Description                                            |
| --------------------------- | -------- | ------------------------------------------------------ |
| `tag`                       | Yes      | The tag of the MCP feature collection version          |
| `stage`                     | Yes      | The name of the stage                                  |
| `mcp-feature-collection-id` | Yes      | The ID of the MCP Feature Collection                   |
| `api-key`                   | Yes      | API key for authentication                             |
| `force`                     | No       | Will not ask for confirmation on deletes or overwrites |
| `wait-for-approval`         | No       | Wait for approval                                      |
| `cloud-url`                 | No       | The URL of the Nitro registry                          |

If you self-host Nitro or use a dedicated hosted instance, you can specify the `cloud-url` input to point to your instance.
