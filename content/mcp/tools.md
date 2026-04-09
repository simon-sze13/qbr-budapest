# MCP tool reference

Tools are registered in **`main.go`** of [cloudera-cloud-factory-mcp](https://github.com/skotnicky/cloudera-cloud-factory-mcp/tree/app-latest) (`app-latest`). Names and behavior may evolve with the branch; this list matches the common **app-latest** layout.

## Client & refresh

| Tool | Description |
|------|-------------|
| `refresh-taikun-client` | Refresh the API client using current environment credentials |

## Virtual clusters

| Tool | Description |
|------|-------------|
| `create-virtual-cluster` | Create a virtual cluster (project) with optional wait |
| `delete-virtual-cluster` | Delete a virtual cluster |
| `list-virtual-clusters` | List virtual clusters in a parent project |

## Catalogs & packages

| Tool | Description |
|------|-------------|
| `catalog-create` | Create a catalog |
| `catalog-list` | List catalogs |
| `catalog-delete` | Delete a catalog |
| `available-apps-list` | List available apps from the package repository |
| `catalog-app-add` | Add an app to a catalog (optional default parameters) |
| `catalog-apps-list` | List apps in a catalog (or all) |
| `catalog-app-params` | Get parameters for a catalog application |
| `catalog-app-defaults-set` | Set default parameters for a catalog app |

## Application instances

| Tool | Description |
|------|-------------|
| `app-install` | Install an application instance |
| `list-apps` | List application instances in a project |
| `get-app` | Get details for an application instance |
| `update-sync-app` | Update values and sync |
| `uninstall-app` | Uninstall an application instance |
| `wait-for-app` | Wait until an application instance is ready |

## Kubernetes projects

| Tool | Description |
|------|-------------|
| `list-projects` | List Kubernetes projects (optional virtual-cluster filter) |
| `create-project` | Create a Kubernetes project |
| `delete-project` | Delete a project |
| `wait-for-project` | Wait for project ready / healthy |
| `get-project-details` | Detailed project status |
| `list-cloud-credentials` | List cloud credentials |
| `list-flavors` | List flavors for a cloud credential |
| `bind-flavors-to-project` | Bind flavors to a project |
| `add-server-to-project` | Add a server (see tool text for flavor hints) |
| `list-servers` | List servers in a project |
| `delete-servers-from-project` | Delete servers from a project |
| `commit-project` | Commit and deploy (initial deploy can take 10–30 minutes) |

## Kubernetes API (in project)

| Tool | Description |
|------|-------------|
| `deploy-kubernetes-resources` | Apply YAML resources |
| `create-kubeconfig` | Create kubeconfig for a project |
| `get-kubeconfig` | Retrieve kubeconfig content |
| `list-kubeconfig-roles` | List kubeconfig roles |
| `list-kubernetes-resources` | List specialized resources |
| `describe-kubernetes-resource` | Describe a resource |
| `delete-kubernetes-resource` | Delete a resource |
| `patch-kubernetes-resource` | Patch a resource with YAML |

For parameter schemas, rely on the **MCP tool definitions** your client shows, or read the corresponding `*Args` structs in the repository source.

[Lab 1: First connection](lab-01-connection.md){ .md-button .md-button--primary }
