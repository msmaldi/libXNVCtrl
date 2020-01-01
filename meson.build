project ('libXNCtrl', [ 'c' ],
  version: '0.1.1')

libXNCtrl_sources = [ 'src/NVCtrl.c' ]

libXNCtrl_dependencies = [
	dependency('xext'),
  dependency('x11')
]

libXNCtrl_static = static_library ('XNVCtrl',
  libXNCtrl_sources,
  dependencies: libXNCtrl_dependencies
)

libXNCtrl_dependency = declare_dependency (
  link_with: libXNCtrl_static,
  include_directories: [ include_directories('./src') ]
)

subdir('samples')
subdir('test')
