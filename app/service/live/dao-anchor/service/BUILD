package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["service.go"],
    importpath = "go-common/app/service/live/dao-anchor/service",
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
    deps = [
        "//app/service/live/dao-anchor/conf:go_default_library",
        "//app/service/live/dao-anchor/dao:go_default_library",
        "//app/service/live/dao-anchor/service/consumer/v1:go_default_library",
        "//app/service/live/dao-anchor/service/v0:go_default_library",
        "//app/service/live/dao-anchor/service/v1:go_default_library",
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
    srcs = [
        ":package-srcs",
        "//app/service/live/dao-anchor/service/consumer/v1:all-srcs",
        "//app/service/live/dao-anchor/service/v0:all-srcs",
        "//app/service/live/dao-anchor/service/v1:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
