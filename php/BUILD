# Protobuf PHP runtime
#
# See also code generation logic under /src/google/protobuf/compiler/php.

load("@rules_pkg//:mappings.bzl", "pkg_files", "strip_prefix")

pkg_files(
    name = "dist_files",
    srcs = glob([
        "ext/google/protobuf/**/*",
        "src/GPBMetadata/Google/Protobuf/**/*.php",
        "src/Google/Protobuf/**/*.php",
        "tests/*.php",
        "tests/*.sh",
        "tests/proto/**/*.proto",
    ]) + [
        "BUILD",
        "README.md",
        "REFCOUNTING.md",
        "composer.json",
        "generate_descriptor_protos.sh",
        "generate_test_protos.sh",
        "release.sh",
        "src/phpdoc.dist.xml",
        "tests/valgrind.supp",
    ],
    prefix = "php",
    strip_prefix = strip_prefix.from_pkg(""),
    visibility = ["//pkg:__pkg__"],
)
