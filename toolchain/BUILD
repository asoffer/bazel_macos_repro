package(default_visibility = ['//visibility:public'])
load(':cc_toolchain_config.bzl', 'cc_toolchain_config')

cc_toolchain_suite(
    name = 'cc',
    toolchains = {
        'darwin_arm64': ':my_toolchain',
    },
)

filegroup(name = 'empty')

cc_toolchain(
    name = 'my_toolchain',
    toolchain_identifier = 'my-toolchain',
    toolchain_config = ':my_toolchain_config',
    all_files = ':empty',
    compiler_files = ':empty',
    dwp_files = ':empty',
    linker_files = ':empty',
    objcopy_files = ':empty',
    strip_files = ':empty',
    supports_param_files = 0,
)

cc_toolchain_config(
    name = 'my_toolchain_config',
)
