project('clippy','c',
  version: '0.1.0',
  meson_version: '>= 0.40.0',
)

config_h = configuration_data()
config_h.set_quoted('GETTEXT_PACKAGE', 'clippy')
configure_file(
  output: 'clippy-config.h',
  configuration: config_h,
)
add_project_arguments([
  '-I' + meson.build_root(),
], language: 'c')

subdir('src')