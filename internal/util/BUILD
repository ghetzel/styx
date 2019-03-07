load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "blackhole.go",
        "doc.go",
        "errors.go",
        "refcount.go",
        "sectionwriter.go",
    ],
    importpath = "github.com/ghetzel/styx/internal/util",
    visibility = ["//github.com/ghetzel/styx:__subpackages__"],
)

go_test(
    name = "go_default_test",
    srcs = ["refcount_test.go"],
    embed = [":go_default_library"],
)
