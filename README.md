[![Test](https://github.com/jfrog/jfrog-ecosystem-integration-env/actions/workflows/test.yml/badge.svg)](https://github.com/jfrog/jfrog-ecosystem-integration-env/actions/workflows/test.yml)
[![Latest Tag](https://badgen.net/github/tag/jfrog/jfrog-ecosystem-integration-env)](https://releases-docker.jfrog.io/artifactory/reg2/jfrog-ecosystem-integration-env/latest)

# JFrog Ecosystem Integration Environment

JFrog Ecosystem integration environment is a Docker image containing all the tools JFrog CLI integrates with and supports.

## Using the Docker Image

This Docker image can be pulled from `releases.jfrog.io` by running the following command:

```
docker pull releases-docker.jfrog.io/jfrog-ecosystem-integration-env:<tag>
```

Running the docker image:

```
docker run -it releases-docker.jfrog.io/jfrog-ecosystem-integration-env
```

## Supported tools

The image is using `apt` and `sdkman` to download the build tools. Note: In the `:latest` tag, the tools versions may change.

Operating system: Ubuntu 20.04.

|  Tool   | Current version |    Package name    |                      Source                      |
| :-----: | :-------------: | :----------------: | :----------------------------------------------: |
|  .NET   |  2.1.x, 3.1.x   | dotnet-sdk-2.1,3.1 | https://packages.microsoft.com/ubuntu/20.04/prod |
|  cURL   |     7.68.x      |        curl        |                  Ubuntu archive                  |
| Docker  |     20.10.x     |       docker       |     https://download.docker.com/linux/ubuntu     |
|   Go    |     1.18.x      |     golang-go      |              https://golang.org/dl               |
| Gradle  |      7.2.x      |       gradle       |          https://sdkman.io/sdks#gradle           |
|   JDK   |     11.0.x      |        tem         |            https://sdkman.io/jdks#tem            |
|   jq    |      1.6.x      |         jq         |                  Ubuntu archive                  |
|  Maven  |      3.8.x      |       maven        |           https://sdkman.io/sdks#maven           |
|  Mono   |    6.12.0.x     |     mono-devel     |  https://download.mono-project.com/repo/ubuntu   |
| MSBuild |     16.6.x      |      msbuild       |  https://download.mono-project.com/repo/ubuntu   |
| NodeJS  |     16.13.x     |       nodejs       |                  Ubuntu archive                  |
|   npm   |      8.1.x      |        npm         |               npm public registry                |
|  NuGet  |     5.6.0.x     |       nuget        |  https://download.mono-project.com/repo/ubuntu   |
|   Pip   |     20.0.x      |    python3-pip     |                  Ubuntu archive                  |
| Pipenv  |    2022.10.x    |       pipenv       |                  Ubuntu archive                  |
| Podman  |      3.3.x      |       podman       |    https://download.opensuse.org/repositories    |
| Poetry  |      1.2.x      |       poetry       |                https://pypi.org/                 |
| Python  |      3.8.x      |    python3-pip     |                  Ubuntu archive                  |
|  Yarn   |     1.22.x      |        yarn        |               npm public registry                |
