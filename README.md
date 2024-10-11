# OSS Management

## Resources Directory
Some notes about what goes in here
## Package Manager Implementations
Each supported package type has some different needs for the Request payload.
### Maven
Needs to have an *entire* `pom.xml` file base64 encoded and added to the `pomxml` property in the input JSON file.
```json
{
  "packageType": "maven",
  "pomdata": "PHByb2plY3QgeG1sbnM9Imh0dHA6Ly9tYXZlbi5hcGFjaGUub3JnL1BPTS80LjAuMCIgeG1sbnM6eHNpPSJodHRwOi8vd3d3LnczLm9yZy8yMDAxL1hNTFNjaGVtYS1pbnN0YW5jZSIKICB4c2k6c2NoZW1hTG9jYXRpb249Imh0dHA6Ly9tYXZlbi5hcGFjaGUub3JnL1BPTS80LjAuMCBodHRwOi8vbWF2ZW4uYXBhY2hlLm9yZy9tYXZlbi12NF8wXzAueHNkIj4KICA8bW9kZWxWZXJzaW9uPjQuMC4wPC9tb2RlbFZlcnNpb24+CiAgPGdyb3VwSWQ+Y29tLmV4YW1wbGU8L2dyb3VwSWQ+CiAgPGFydGlmYWN0SWQ+bXktYXBwPC9hcnRpZmFjdElkPgogIDxwYWNrYWdpbmc+amFyPC9wYWNrYWdpbmc+CiAgPHZlcnNpb24+MS4wLVNOQVBTSE9UPC92ZXJzaW9uPgogIDxuYW1lPm15LWFwcDwvbmFtZT4KICA8dXJsPmh0dHA6Ly9tYXZlbi5hcGFjaGUub3JnPC91cmw+CiAgPGRlcGVuZGVuY2llcz4KICAgIDxkZXBlbmRlbmN5PgogICAgICA8Z3JvdXBJZD5qdW5pdDwvZ3JvdXBJZD4KICAgICAgPGFydGlmYWN0SWQ+anVuaXQ8L2FydGlmYWN0SWQ+CiAgICAgIDx2ZXJzaW9uPjMuOC4xPC92ZXJzaW9uPgogICAgICA8c2NvcGU+dGVzdDwvc2NvcGU+CiAgICA8L2RlcGVuZGVuY3k+CiAgPC9kZXBlbmRlbmNpZXM+CjwvcHJvamVjdD4=",
  "requestor": "tomj@jfrog.com",
  "applicationId": "1234"
}
```
## TODOs
* Check for the presence of the requested library in the `scans-<packagetype>-local` repo in target Artifcatory instance