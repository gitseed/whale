# whale
A program for constructing docker images while keeping your sanity

Features:

* Roles
* Jinja2 template files
* Implicit `set -euo pipefail ;` before each RUN
* Abstraction layers over common use cases, such as zip, COPY, unzip

Plan:

* Phase one: Just docker command passthroughs and "adaptive copy"
* Adaptive copy: A synthetic build context is created with only the files needed!
