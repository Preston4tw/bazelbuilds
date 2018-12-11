load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
load("@bazel_tools//tools/build_defs/repo:git.bzl", "new_git_repository")

http_archive(
    name = "lzfse",
    build_file = "//third_party:lzfse.BUILD",
    sha256 = "a15063c0b0b1400791f0767c143367f8d70b6e3fdda78c2e6d8b9c870dc4a7db",
    urls = ["https://github.com/lzfse/lzfse/tarball/e634ca5"],
    strip_prefix = "lzfse-lzfse-e634ca5",
    type = "tar.gz",
)

new_git_repository(
    name = "zlib",
    build_file = "//third_party:zlib.BUILD",
    remote = "https://github.com/madler/zlib",
    commit = "cacf7f1d4e3d44d871b605da3b647f07d718623f",
)