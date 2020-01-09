project ('libXNVCtrl', [ 'c' ],
    version: '0.1.2')

libXNVCtrl_sources = [ 'src/NVCtrl.c' ]

libXNVCtrl_dependencies = [
	dependency('xext'),
    dependency('x11')
]

libXNVCtrl_static = static_library ('XNVCtrl',
    libXNVCtrl_sources,
    dependencies: libXNVCtrl_dependencies
)

libXNVCtrl_dependency = declare_dependency (
    link_with: libXNVCtrl_static,
    include_directories: [ include_directories('./src') ]
)

subdir('samples')
