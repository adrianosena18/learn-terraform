# Assignment examples

In these examples, multiple resource groups are created. They **must** have a unique `name` and identifier when not using `count` or `for_each`.
On working out this example, you may use the same name and identifier.

## Example 1

```hcl
resource "azurerm_resource_group" "example-1" {
  name     = "example-1"
  location = "West Europe"
}

resource "azurerm_resource_group" "example-2" {
  name     = "example-2"
  location = "West Europe"
}
```

## Example 2

```hcl
resource "azurerm_resource_group" "example-1" {
  name     = "example-1"
  location = "westeurope"
}

resource "azurerm_resource_group" "example-2" {
  name     = "example-2"
  location = "easteurope"
}
```

## Example 3

```hcl
resource "azurerm_resource_group" "example-1" {
  name     = "my_first_resource_group"
  location = "westeurope"
}

resource "azurerm_resource_group" "example-2" {
  name     = "my_second_resource_group"
  location = "easteurope"
}
```
