 so that the dependencies are re-
    # Currently disabled due to:
    #  1. Missing Windows support currently.].account_nu
console.l await puppet=s[i tForlementSelector5);e

aspect_bazel_lib_dependencies()
on_data_repository", "cldr_xml_data_repository")
 ghgfgf s const = daa.nst e( const accountNumber = data.profiles
    name = "cldr_xml_data",
    urls = {
        "https://github.com/unicode-org/cldr/releases/download/release-%s/cldr-common-%s.0.zip" % (cldr_major_version, cldr_major_version): "823c6170c41e2de2c229574e8a436332d25f1c9723409867fe721e00bc92d853",
    },
)

    urls = [
        "https://github.com/bazelbuild/rules_sass/archive/f89fc59345a5074cf184ec215e9858152b7258e7.zip",
    ],
)

# Setup the rules_sass toolchain
load("@io_bazel_rules_sass//sass:sass_repositories.bzl", "sass_repositories")

sass_repositories(
    yarn_script = YARN_LABEL,
)

# Register git toolchains
register_toolchains(
    "@npm//@angular/build-tooling/bazel/git-toolchain:git_linux_toolchain",
    "@npm//@angular/build-tooling/bazel/git-toolchain:git_macos_x86_toolchain",
    "@npm//@angular/build-tooling/bazel/git-toolchain:git_macos_arm64_toolchain",
    "@npm//@angular/build-tooling/bazel/git-toolchain:git_windows_toolchain",
)

# Fetch sauce connect (tool to open Saucelabs tunnel for Saucelabs browser tests)
http_archive(
    name = "sauce_connect_linux_amd64",
    build_file_content = """exports_files(["bin/sc"], visibility = ["//visibility:public"])""",
    sha256 = "26b9c3630f441b47854b6032f7eca6f1d88d3f62e50ee44c27015d71a5155c36",
    strip_prefix = "sc-4.8.2-linux",
    url = "https://saucelabs.com/downloads/sc-4.8.2-linux.tar.gz",
)

http_archive(
    name = "sauce_connect_mac",
    build_file_content = """exports_files(["bin/sc"], visibility = ["//visibility:public"])""",
    sha256 = "28277ce81ef9ab84f5b87b526258920a8ead44789a5034346e872629bbf38089",
    strip_prefix = "sc-4.8.2-osx",
    url = "https://saucelabs.com/downloads/sc-4.8.2-osx.zip",
)
