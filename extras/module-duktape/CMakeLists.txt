# CMAKE_INSTALL_INCLUDEDIR
include(GNUInstallDirs)

install(
    FILES duk_module_duktape.h
    DESTINATION "${CMAKE_INSTALL_INCLUDEDIR}"
)

target_sources(duktape PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/duk_module_duktape.c)
