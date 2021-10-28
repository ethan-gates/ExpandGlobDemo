load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")

git_repository(
    name = "build_bazel_rules_ios",
    remote = "https://github.com/bazel-ios/rules_ios.git",
    branch = "master",
)

#local_repository(
#    name = "build_bazel_rules_ios",
#    path = "/Users/egates/Documents/code/oss-rules-ios/rules_ios",
#)

load(
    "@build_bazel_rules_ios//rules:repositories.bzl",
    "rules_ios_dependencies"
)

rules_ios_dependencies()

load(
    "@build_bazel_rules_apple//apple:repositories.bzl",
    "apple_rules_dependencies",
)

apple_rules_dependencies()

load(
    "@build_bazel_rules_swift//swift:repositories.bzl",
    "swift_rules_dependencies",
)

swift_rules_dependencies()

load(
    "@build_bazel_apple_support//lib:repositories.bzl",
    "apple_support_dependencies",
)

apple_support_dependencies()


git_repository(
  name = "com_google_protobuf",
  remote = "https://github.com/protocolbuffers/protobuf",
  commit = "51405b6b92c2070c8edea1b44c6770e00f7027be",
  shallow_since = "1628094119 +0300"
)
load(
  "@com_google_protobuf//:protobuf_deps.bzl",
  "protobuf_deps",
)

protobuf_deps()
