---
layout: "hcloud"
page_title: "Hetzner Cloud: hcloud_datacenter"
sidebar_current: "docs-hcloud-datasource-datacenter"
description: |-
  Provides details about a specific Hetzner Cloud Datacenter.
---
# Data Source: hcloud_datacenter
Provides details about a specific Hetzner Cloud Datacenter.
Use this resource to get detailed information about specific datacenter.

## Example Usage
```hcl
data "hcloud_datacenter" "ds_1" {
  name = "fsn1-dc8"
}
data "hcloud_datacenter" "ds_2" {
  id = 4
}
```
## Argument Reference
- `id` - (Optional, string) ID of the datacenter.
- `name` - (Optional, string) Name of the datacenter.

## Attributes Reference
- `id` - (int) Unique ID of the datacenter.
- `name` - (string) Name of the datacenter.
- `description` - (string) Description of the datacenter.
- `location` - (map) Physical datacenter location.
- `supported_server_type_ids` - (list) List of server types supported by the datacenter.
- `available_server_type_ids` - (list) List of available server types.
