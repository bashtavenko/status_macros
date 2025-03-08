load("@rules_cc//cc:defs.bzl", "cc_library")

package(default_visibility = ["//visibility:public"])

cc_test(
    name = "status_macros_test",
    srcs = ["status_macros_test.cc"],
    deps = [
        "@absl//absl/status",
        "@absl//absl/status:statusor",
        "@googletest//:gtest_main",
        "@status_macros",
    ],
)
