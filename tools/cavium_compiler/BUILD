package(default_visibility = ["//visibility:public"])

cc_toolchain_suite(
  name = "toolchain",
  # target_cpu | compiler
  toolchains = {
    'mips64|compiler':':cc-compiler-mips64',
    "local|compiler": ":cc-compiler-local",
  },
)

filegroup(
    name = "empty",
    srcs = [],
)

filegroup(
    name = "mips64_all_files",
    srcs = [
    "@cavium_compiler//:compiler_pieces",
  ],
)

cc_toolchain(
    name = "cc-compiler-local",
    all_files = ":empty",
    compiler_files = ":empty",
    cpu = "local",
    dwp_files = ":empty",
    dynamic_runtime_libs = [":empty"],
    linker_files = ":empty",
    objcopy_files = ":empty",
    static_runtime_libs = [":empty"],
    strip_files = ":empty",
    supports_param_files = 1,
)


cc_toolchain(
  name = 'cc-compiler-mips64',
  all_files = ':mips64_all_files',
  compiler_files = ':mips64_all_files',
  cpu = 'mips64',
  dwp_files = ':empty',
  dynamic_runtime_libs = [':empty'],
  linker_files = ':mips64_all_files',
  objcopy_files = 'mips64_all_files',
  static_runtime_libs = [':empty'],
  strip_files = 'mips64_all_files',
  supports_param_files = 1,
)
