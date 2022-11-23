project('erupted', 'd')

src = files(
  'source/erupted/functions.d',
  'source/erupted/types.d',
)

lib = library('erupted', src,
  include_directories : ['./source']
)

erupted_dep = declare_dependency(
  include_directories : ['./source'],
  link_with : lib,
)

meson.override_dependency('erupted', erupted_dep)