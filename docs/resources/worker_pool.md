---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "spacelift_worker_pool Resource - terraform-provider-spacelift"
subcategory: ""
description: |-
  spacelift_worker_pool represents a worker pool assigned to the Spacelift account.
---

# spacelift_worker_pool (Resource)

`spacelift_worker_pool` represents a worker pool assigned to the Spacelift account.

## Example Usage

```terraform
resource "spacelift_worker_pool" "k8s-core" {
  name        = "Main worker"
  csr         = filebase64("/path/to/csr")
  description = "Used for all type jobs"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- **name** (String) name of the worker pool

### Optional

- **csr** (String, Sensitive) certificate signing request in base64
- **description** (String) description of the worker pool
- **id** (String) The ID of this resource.

### Read-Only

- **config** (String, Sensitive) credentials necessary to connect WorkerPool's workers to the control plane
- **private_key** (String, Sensitive) private key in base64


