# Dockerfile Best Practices
This repository demonstrates common issues in Dockerfiles and provides improved versions.

## Problem:
The original `Dockerfile` uses `ubuntu:latest`, resulting in inconsistent builds.  The `COPY` command could be optimized, and a missing health check leaves room for improvement.

## Solution:
The improved `Dockerfile.fixed` addresses these problems by:
1. Specifying a version for Ubuntu (e.g., `ubuntu:22.04`)
2. Optimizing `COPY` for better efficiency
3. Adding a basic health check command.