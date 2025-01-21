# Unpredictable Docker Builds Due to `ubuntu:latest`

This example demonstrates a common issue with Dockerfiles: using `ubuntu:latest`.  Using `latest` means your build environment will change unexpectedly as new versions of Ubuntu are released, which is bad for reproducibility.

This repo contains two files:

* `Dockerfile`: A Dockerfile using `ubuntu:latest`.  This exhibits the problem.
* `Dockerfile_solution`: A corrected Dockerfile, using a specific Ubuntu version.