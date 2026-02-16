# kind + helmfile example

## Prerequisites

- mise
- docker (for kind to be able to run)

## Deploy

```bash
mise run deploy-dev
# will setup the kind cluster (if needed) and then deploy everything specified in the helmfile for the "dev" environment
```

To check if it worked you should be able to access: [example.localtest.me](http://example.localtest.me) and be greeted with a html page that shows the rendered [charts/example-app/files/index.html](./charts/example-app/files.index.html).

> [!NOTE]
> You might have to wait a few seconds before the page is accessible.

## Destroy

```bash
mise run delete-kind-cluster
# destroys the kind cluster (if needed)
```

