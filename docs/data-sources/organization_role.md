---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "awx_organization_role Data Source - terraform-provider-awx"
subcategory: ""
description: |-
  Data source for an organization role
---

# awx_organization_role (Data Source)

Data source for an organization role

## Example Usage

```terraform
data "awx_organization" "example" {
  name = "My Organization"
}


data "awx_organization_role" "example" {
  name            = "Admin"
  organization_id = awx_organization.example.id
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `organization_id` (Number) The ID of the organization

### Optional

- `id` (Number) The ID of the organization role
- `name` (String) The name of the organization role