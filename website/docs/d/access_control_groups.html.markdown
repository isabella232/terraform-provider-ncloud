---
layout: "ncloud"
page_title: "NCLOUD: ncloud_access_control_groups"
sidebar_current: "docs-ncloud-datasource-access-control-groups"
description: |-
  Get access control group list
---

# Data Source: ncloud_access_control_groups

When creating a server instance (VM), you can add an access control group (ACG) that you specified to set firewalls. This data source gets a list of access control groups necessary to set firewalls.

## Example Usage

```hcl
data "ncloud_access_control_groups" "acg" {}
```

## Argument Reference

The following arguments are supported:

* `configuration_no_list` - (Optional) List of ACG configuration numbers you want to get
* `is_default_group` - (Optional) Indicates whether to get default groups only
* `name` - (Optional) Name of the ACG you want to get
* `output_file` - (Optional) The name of file that can save data source after running `terraform plan`.

## Attributes Reference

* `access_control_groups` - A List of access control group configuration_no.
