# Google C++ Status Macros

This repository contains a [bazel](https://bazel.build) build target for Google C++ status macros,
redistributed from [mediapipe](https://github.com/google/mediapipe).

## Setup

### MODULE.bzl


```
http_archive = use_repo_rule("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "status_macros",
    strip_prefix = "status_macros-1.0.1",
    urls = ["https://github.com/bashtavenko/status_macros/archive/refs/tags/v1.0.1.tar.gz"],
)
```

### BUILD

Add `"@status_macros"` to BUILD deps for targets that use this.

## Usage

Add `#include "status_macros.h"` to your source.

See [RETURN_IF_ERROR](https://github.com/jimrogerz/status_macros/blob/main/status_macros.h#L29) and [ASSIGN_OR_RETURN](https://github.com/jimrogerz/status_macros/blob/main/status_macros.h#L91).
