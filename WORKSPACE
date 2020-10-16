load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "rules_foreign_cc",
    strip_prefix = "rules_foreign_cc-master",
    url = "https://github.com/bazelbuild/rules_foreign_cc/archive/master.zip",
)

load("@rules_foreign_cc//:workspace_definitions.bzl", "rules_foreign_cc_dependencies")

rules_foreign_cc_dependencies()

all_content = """filegroup(name = "testu01_all", srcs = glob(["**"]), visibility = ["//visibility:public"])"""

http_archive(
    name = "testu01",
    build_file_content = all_content,
    sha256 = "bc1d1dd2aea7ed3b3d28eaad2c8ee55913f11ce67aec8fe4f643c1c0d2ed1cac",
    strip_prefix = "TestU01-1.2.3",
    urls = ["http://simul.iro.umontreal.ca/testu01/TestU01.zip"],
)
