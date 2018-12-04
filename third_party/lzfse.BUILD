# licenses(['notice'])

package(default_visibility = ['//visibility:public'])

filegroup(
    name = "lzfse_sources",
    srcs = [
        "src/lzfse_decode.c",
        "src/lzfse_decode_base.c",
        "src/lzfse_encode.c",
        "src/lzfse_encode_base.c",
        "src/lzfse_fse.c",
        "src/lzvn_decode_base.c",
        "src/lzvn_encode_base.c",
        "src/lzfse_internal.h",
        "src/lzfse_fse.h",
        "src/lzvn_encode_base.h",
        "src/lzvn_decode_base.h",
        "src/lzfse_tunables.h",
        "src/lzfse_encode_tables.h",
    ],
)

# https://docs.bazel.build/versions/master/be/c-cpp.html#cc_library
cc_library(
    name = "lzfse",
    srcs = [":lzfse_sources"],
    hdrs = [
        "src/lzfse.h",
    ],
)

# https://docs.bazel.build/versions/master/be/c-cpp.html#cc_binary
cc_binary(
    name = "lzfse_cli",
    srcs = ["src/lzfse_main.c"],
    deps = [":lzfse"],
)