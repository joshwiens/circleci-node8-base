<div align="center">
  <img width="200" height="200"
    src="https://cdn.worldvectorlogo.com/logos/circleci.svg">
  <a href="https://docker.com">
    <img width="200" height="200" vspace="" hspace="25"
      src="https://cdn.worldvectorlogo.com/logos/docker.svg">
  </a>
  <h1>CircleCI 2.0 Node 8.2 Build container</h1>
  <p>Docker Repository for my NodeJS CircleCI 2.0 build & deployment Image.<p>
</div>

### Usage
```bash
# config.yml
    docker:
      - image: d3vaint0ne/circleci-node8-base
```

Essentially it's circleci/node:8.2.1 + NVM + Google Cloud SDK. The SDK is not initialized in this build, this is done during the consuming CI run using secure environment variables ( see the [gpc docs](https://circleci.com/docs/2.0/google-container-engine/) ).

The container does not have a headless browser configuration ( Jest 4 life ) 
