CircleCI Build Dockerfile
=========================

Features:

    * Node 8 (based on circleci/node:8)
    * Docker command line tools
    * awscli: The `aws` command line tool
    * Python 3.6
    * Git LFS
    * `/home/circleci/checkout.sh` script that uses `git lfs clone` instead of `git clone`, for faster checkout of Git LFS content.

Fast LFS Checkout
-----------------
To use the fast `git lfs clone` checkout command, replace the `checkout` command in your CircleCI configuration file with:

```yaml
      - run: /home/circleci/checkout.sh
```
