load("@bazel_skylib//:bzl_library.bzl", "bzl_library")
load("//rust:rust.bzl", "error_format")

exports_files(["LICENSE"])

bzl_library(
    name = "rules",
    srcs = [
        ":workspace.bzl",
    ],
    visibility = ["//visibility:public"],
)

# This setting may be changed from the command line to generate machine readable errors.
error_format(
    name = "error_format",
    build_setting_default = "human",
    visibility = ["//visibility:public"],
)
