load("@rules_foreign_cc//tools/build_defs:configure.bzl", "configure_make")

configure_make(
    name = "testu01_configure",
    configure_in_place = True,
    lib_source = "@testu01//:testu01_all",
    out_lib_dir = "lib",
    static_libraries = ["libmylib.a"],
    visibility = ["//visibility:public"],
)
