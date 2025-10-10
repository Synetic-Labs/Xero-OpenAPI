Run to pull from main branch and remove recursive references from the spec.

```bash
docker run --rm -v "$(pwd):/spec" redocly/cli bundle https://raw.githubusercontent.com/XeroAPI/Xero-OpenAPI/refs/heads/master/xero_accounting.yaml --output /spec/xero_accounting.yaml --dereferenced
```