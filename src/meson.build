valasample_sources = [
  'main.vala',
  'window.vala',
]

valasample_deps = [
  dependency('gio-2.0', version: '>= 2.50'),
  dependency('gtk+-3.0', version: '>= 3.22'),
]

gnome = import('gnome')

valasample_sources += gnome.compile_resources('valasample-resources',
  'valasample.gresource.xml',
  c_name: 'valasample'
)

executable('valasample', valasample_sources,
  vala_args: '--target-glib=2.50',  dependencies: valasample_deps,
  install: true,
)
