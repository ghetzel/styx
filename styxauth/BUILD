load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "auth.go",
        "doc.go",
        "socket.go",
        "tls.go",
    ],
    importpath = "github.com/ghetzel/styx/styxauth",
    visibility = ["//visibility:public"],
    deps = [
        "//github.com/ghetzel/styx:go_default_library",
    ],
)
