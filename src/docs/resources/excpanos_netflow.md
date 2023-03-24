---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "excpanos_netflow Resource - src"
subcategory: ""
description: |-
  
---

# excpanos_netflow (Resource)





<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `name` (String) The administrative Netflow's name
- `server` (Block List, Min: 1) The server to send the netflow (see [below for nested schema](#nestedblock--server))

### Optional

- `active_timeout` (Number) Minutes before a flow is considered inactive
- `template_refresh_rate` (Block Set) Netflow template refresh rate (see [below for nested schema](#nestedblock--template_refresh_rate))

### Read-Only

- `id` (String) The ID of this resource.

<a id="nestedblock--server"></a>
### Nested Schema for `server`

Required:

- `hostname` (String) The hostname of the server
- `name` (String) The name of the server
- `port` (Number) The port of the server


<a id="nestedblock--template_refresh_rate"></a>
### Nested Schema for `template_refresh_rate`

Optional:

- `minutes` (Number) Minutes beetwen each refresh
- `paquets` (Number) Seconds beetwen each refresh

