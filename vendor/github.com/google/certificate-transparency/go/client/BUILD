load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["logclient.go"],
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/google/certificate-transparency/go:go_default_library",
        "//vendor/github.com/mreiferson/go-httpclient:go_default_library",
        "//vendor/golang.org/x/net/context:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
