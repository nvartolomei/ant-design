---
category: Components
type: Navigation
title: Breadcrumb
---

A breadcrumb displays the current location within a hierarchy. It allows going back to states higher up within the hierarchy.

## When To Use

- When the system has more than two layers in a hierarchy.
- When you need to inform the user of where they are.
- When the user may need to navigate back to a higher level When the application has multi-layer architecture.

## API

```html
<Breadcrumb>
  <Breadcrumb.Item>Home</Breadcrumb.Item>
  <Breadcrumb.Item>Application Center</Breadcrumb.Item>
  <Breadcrumb.Item>Application List</Breadcrumb.Item>
  <Breadcrumb.Item>An Application</Breadcrumb.Item>
</Breadcrumb>
```

| Property      | Description                              | Type              |  Optional | Default |
|-----------|-----------------------------------|-----------------|---------|--------|
| routes    | The routing stack information of router | Array             |         | -      |
| params    | Routing parameter                        | Object            |         | -      |
| separator | Custom separator                      | String or Element |         | '/'    |
| itemRender | Custom item renderer | (route, params, routes, paths) => React.ReactNode | | - |

> `linkRender` and `nameRender` were removed after `antd@2.0`, please use `itemRender` instead.
