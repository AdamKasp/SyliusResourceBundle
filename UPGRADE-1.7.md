# UPGRADE FROM `v1.6.*` TO `v1.7.0`

* **BC BREAK**: Edit your fos_rest config to enable the body listener as following:
```yaml
fos_rest:
    # [...]
    body_listener:
        enabled: true 
```

* **BC BREAK**: `ViewHandler` constructor now requires `FOS\RestBundle\View\ConfigurableViewHandlerInterface` as first argument instead of 
    `FOS\RestBundle\View\ViewHandler`.
