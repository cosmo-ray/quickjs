This is a quickjs fork for YIRL

it include:
- fix that add -fPIC in th CFLAGS
- some fixes in order to include quickjs.h with gcc 9
- an ugly hack js_check_stack_overflow to use intptr_t instead of size_t for comparaison because on mymachine sometime size was negative.
- another hack so I can link libtcc.a and libquickjs.a with the same library (because a symbole was redeclared)

The main documentation is in doc/quickjs.pdf or doc/quickjs.html.
