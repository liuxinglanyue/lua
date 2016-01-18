cmake_minimum_required(VERSION 3.3)
project(lua_5_2_2)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES src/lapi.h src/lapi.c src/lauxlib.c src/lauxlib.h
        src/lbaselib.c src/lbitlib.c src/lcode.c src/lcode.h src/lcorolib.c
        src/lctype.c src/lctype.h src/ldblib.c src/ldebug.c src/ldebug.h
        src/ldo.c src/ldo.h src/ldump.c src/lfunc.c src/lfunc.h src/lgc.c
        src/lgc.h src/linit.c src/liolib.c src/llex.c src/llex.h
        src/llimits.h src/lmathlib.c src/lmem.c src/lmem.h src/loadlib.c
        src/lobject.c src/lobject.h src/lopcodes.h src/lopcodes.c src/loslib.c
        src/lparser.c src/lparser.h src/lstate.c src/lstate.h src/lstring.c
        src/lstring.h src/lstrlib.c src/ltable.c src/ltable.h src/ltablib.c
        src/ltm.c src/ltm.h src/lua.c src/lua.h src/lua.hpp src/luac.c
        src/luaconf.h src/lualib.h src/lundump.c src/lundump.h src/lvm.c
        src/lvm.h src/lzio.c src/lzio.h)
add_executable(lua_5_2_2 ${SOURCE_FILES})