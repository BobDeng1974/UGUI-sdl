add_executable(sdl_app
  ../UGUI/ugui.c sdl.c)
find_package(SDL)
target_include_directories(sdl_app PRIVATE ${SDL_INCLUDE_DIR} . ../UGUI )
target_link_libraries(sdl_app ${SDL_LIBRARY}) 

