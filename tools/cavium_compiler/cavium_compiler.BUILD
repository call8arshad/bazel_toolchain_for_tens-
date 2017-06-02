package(default_visibility = ['//visibility:public'])

filegroup(
  name = 'gcc',
  srcs = [
    'bin/mips64-octeon-linux-gnu-gcc',
  ],
)

filegroup(
  name = 'ar',
  srcs = [
    'bin/mips64-octeon-linux-gnu-ar',
  ],
)

filegroup(
  name = 'ld',
  srcs = [
    'bin/mips64-octeon-linux-gnu-ld',
  ],
)

filegroup(
  name = 'nm',
  srcs = [
    'bin/mips64-octeon-linux-gnu-nm',
  ],
)

filegroup(
  name = 'objcopy',
  srcs = [
    'bin/mips64-octeon-linux-gnu-objcopy',
  ],
)

filegroup(
  name = 'objdump',
  srcs = [
    'bin/mips64-octeon-linux-gnu-objdump',
  ],
)

filegroup(
  name = 'strip',
  srcs = [
    'bin/mips64-octeon-linux-gnu-strip',
  ],
)

filegroup(
  name = 'as',
  srcs = [
    'bin/mips64-octeon-linux-gnu-as',
  ],
)

filegroup(
  name = 'compiler_pieces',
  srcs = glob([
    'mips64-octeon-linux-gnu/**',
    'libexec/**',
    'lib/gcc/mips64-octeon-linux-gnu/**',
    'include/**',
  ]),
)

filegroup(
  name = 'compiler_components',
  srcs = [
    ':gcc',
    ':ar',
    ':ld',
    ':nm',
    ':objcopy',
    ':objdump',
    ':strip',
    ':as',
  ],
)
