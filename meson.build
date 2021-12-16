project('lunarbase', 'c',
  version : '0.1',
  default_options : ['warning_level=3'])


libuv_dep = dependency('libuv', fallback: ['libuv', 'libuv_dep'])
lua_dep = dependency('lua', fallback: ['lua', 'lua_dep'])

exe = executable('lunarbase', 'src/main.c',
  dependencies : [libuv_dep, lua_dep],
  install : true)

test('basic', exe)
