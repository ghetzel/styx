load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "auth.go",
        "conn.go",
        "doc.go",
        "file.go",
        "request.go",
        "server.go",
        "session.go",
        "stack.go",
        "walk.go",
        "wstat.go",
    ],
    importpath = "github.com/ghetzel/styx",
    visibility = ["//visibility:public"],
    deps = [
        "//github.com/ghetzel/styx/internal/qidpool:go_default_library",
        "//github.com/ghetzel/styx/internal/styxfile:go_default_library",
        "//github.com/ghetzel/styx/internal/sys:go_default_library",
        "//github.com/ghetzel/styx/internal/threadsafe:go_default_library",
        "//github.com/ghetzel/styx/internal/tracing:go_default_library",
        "//github.com/ghetzel/styx/internal/util:go_default_library",
        "//github.com/ghetzel/styx/styxproto:go_default_library",
        "//aqwari.net/retry:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "example_stack_test.go",
        "example_test.go",
        "server_test.go",
    ],
    data = ["//github.com/ghetzel/styx/styxproto:testdata"],
    embed = [":go_default_library"],
    deps = [
        "//github.com/ghetzel/styx/internal/netutil:go_default_library",
        "//github.com/ghetzel/styx/styxproto:go_default_library",
    ],
)
