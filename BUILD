load("@io_bazel_rules_jsonnet//jsonnet:jsonnet.bzl", "jsonnet_library", "jsonnet_to_json")

jsonnet_library(
    name = "sit-env",
    srcs = [
        "sit-env.jsonnet",
    ],
)

jsonnet_to_json(
    name = "app1",
    src = "app1.jsonnet",
    outs = ["app1.json"],
    deps = [":sit-env"],
)
