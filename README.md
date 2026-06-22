# DockerCacheRepo

Starter project for the **Docker layer-caching** GitHub Actions lab.

This repository contains a minimal Dockerized Node.js app. The `Dockerfile`
installs dependencies in a separate layer from the application source, so
intelligent layer caching can reuse the dependency layer across builds. Copy
these files into your own repository, then add the build workflow at
`.github/workflows/docker-cache-ci.yml` as described in the lab instructions.

```
DockerCacheRepo/
├── Dockerfile
├── package.json
└── app.js
```

> Note: This repo intentionally does **not** include the workflow file —
> creating it is part of the lab task.
