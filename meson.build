project('game', 'cpp',
  version : '0.1',
  default_options : ['warning_level=3',
                     'cpp_std=c++14'])

gl = dependency('gl', method: 'pkg-config', required: true)
glu = dependency('glu')
glut = dependency('GLUT', method: 'cmake')

exe = executable('game', 'game.cpp',
  dependencies: [
	gl, glu, glut
  ],
  install : true)

test('basic', exe)
