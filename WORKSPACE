load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "google_jsonnet_go",
    sha256 = "4fd04d0c9e38572ef388d28ea6b1ac151b8a9a5026ff94e3a68bdbc18c4db38a",
    strip_prefix = "go-jsonnet-0.17.0",
    urls = ["https://github.com/google/go-jsonnet/archive/refs/tags/v0.17.0.tar.gz"],
)

http_archive(
    name = "io_bazel_rules_jsonnet",
    sha256 = "7f51f859035cd98bcf4f70dedaeaca47fe9fbae6b199882c516d67df416505da",
    strip_prefix = "rules_jsonnet-0.3.0",
    urls = ["https://github.com/bazelbuild/rules_jsonnet/archive/0.3.0.tar.gz"],
)

load("@io_bazel_rules_jsonnet//jsonnet:jsonnet.bzl", "jsonnet_repositories")

jsonnet_repositories()

load("@google_jsonnet_go//bazel:repositories.bzl", "jsonnet_go_repositories")

jsonnet_go_repositories()

load("@google_jsonnet_go//bazel:deps.bzl", "jsonnet_go_dependencies")

jsonnet_go_dependencies()