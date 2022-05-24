testapp_sources = [
  'main.vala',
  'window.vala',
  'application.vala',
]

testapp_deps = [
  dependency('libadwaita-1', version: '>= 1.0'),
]

gnome = import('gnome')

testapp_sources += gnome.compile_resources('testapp-resources',
  'testapp.gresource.xml',
  c_name: 'testapp'
)

executable('testapp', testapp_sources,
  vala_args: '--target-glib=2.50',  dependencies: testapp_deps,
  install: true,
)
