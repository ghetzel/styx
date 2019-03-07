load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "group_go17.go",
        "group_oldgo.go",
        "owner.go",
        "owner_fallback.go",
        "owner_plan9.go",
        "owner_unix.go",
    ],
    importpath = "github.com/ghetzel/styx/internal/sys",
    visibility = ["//github.com/ghetzel/styx:__subpackages__"],
    deps = [
        "//github.com/ghetzel/styx/styxproto:go_default_library",
    ],
)
