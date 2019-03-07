load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

filegroup(
    name = "testdata",
    srcs = glob(["testdata/*.9p"]),
    visibility = ["//github.com/ghetzel/styx:__subpackages__"],
)

go_library(
    name = "go_default_library",
    srcs = [
        "decoder.go",
        "doc.go",
        "encoder.go",
        "enum.go",
        "errors.go",
        "limits.go",
        "pack.go",
        "parse.go",
        "proto.go",
        "qid.go",
        "stat.go",
        "verify.go",
    ],
    importpath = "github.com/ghetzel/styx/styxproto",
    visibility = ["//visibility:public"],
)

go_test(
    name = "go_default_test",
    srcs = [
        "encoding_test.go",
        "example_test.go",
        "malformed_test.go",
        "styxproto_test.go",
    ],
    data = [":testdata"],
    embed = [":go_default_library"],
)
