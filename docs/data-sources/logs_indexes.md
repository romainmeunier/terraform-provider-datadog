---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "datadog_logs_indexes Data Source - terraform-provider-datadog"
subcategory: ""
description: |-
  Use this data source to list several existing logs indexes for use in other resources.
---

# datadog_logs_indexes (Data Source)

Use this data source to list several existing logs indexes for use in other resources.

## Example Usage

```terraform
data "datadog_logs_indexes" "test" {}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Read-Only

- **id** (String) The ID of this resource.
- **logs_indexes** (List of Object) List of logs indexes (see [below for nested schema](#nestedatt--logs_indexes))

<a id="nestedatt--logs_indexes"></a>
### Nested Schema for `logs_indexes`

Read-Only:

- **daily_limit** (Number)
- **exclusion_filter** (List of Object) (see [below for nested schema](#nestedobjatt--logs_indexes--exclusion_filter))
- **filter** (List of Object) (see [below for nested schema](#nestedobjatt--logs_indexes--filter))
- **name** (String)
- **retention_days** (Number)

<a id="nestedobjatt--logs_indexes--exclusion_filter"></a>
### Nested Schema for `logs_indexes.exclusion_filter`

Read-Only:

- **filter** (List of Object) (see [below for nested schema](#nestedobjatt--logs_indexes--exclusion_filter--filter))
- **is_enabled** (Boolean)
- **name** (String)

<a id="nestedobjatt--logs_indexes--exclusion_filter--filter"></a>
### Nested Schema for `logs_indexes.exclusion_filter.filter`

Read-Only:

- **query** (String)
- **sample_rate** (Number)



<a id="nestedobjatt--logs_indexes--filter"></a>
### Nested Schema for `logs_indexes.filter`

Read-Only:

- **query** (String)

