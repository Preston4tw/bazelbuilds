# This is just a rule serving as a top level dependency we can build to ensure
# all of the third party deps build
genrule(
    name = "dummy_target",
    srcs = [
        "@lzfse//:lzfse",
        "@lzfse//:lzfse_cli",
    ],
    outs = [
        "dummy.txt",
    ],
    cmd = "ls / > $@",
)