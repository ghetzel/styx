load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "dir.go",
        "dumb.go",
        "file.go",
        "mode.go",
        "seeker.go",
    ],
    importpath = "github.com/ghetzel/styx/internal/styxfile",
    visibility = ["//github.com/ghetzel/styx:__subpackages__"],
    deps = [
        "//github.com/ghetzel/styx/internal/qidpool:go_default_library",
        "//github.com/ghetzel/styx/internal/sys:go_default_library",
        "//github.com/ghetzel/styx/styxproto:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "file_test.go",
        "mode_test.go",
    ],
    embed = [":go_default_library"],
    deps = [
        "//github.com/ghetzel/styx/internal/qidpool:go_default_library",
        "//github.com/ghetzel/styx/styxproto:go_default_library",
    ],
)
