load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["pool.go"],
    importpath = "github.com/ghetzel/styx/internal/qidpool",
    visibility = ["//github.com/ghetzel/styx:__subpackages__"],
    deps = [
        "//github.com/ghetzel/styx/internal/threadsafe:go_default_library",
        "//github.com/ghetzel/styx/styxproto:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["pool_test.go"],
    embed = [":go_default_library"],
    deps = ["//github.com/ghetzel/styx/styxproto:go_default_library"],
)
