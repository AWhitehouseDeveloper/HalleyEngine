cmake_minimum_required (VERSION 3.10)

project (HalleyEngine)

set(HALLEY_PROJECT_EMBED 1)
set(HALLEY_PATH ${CMAKE_CURRENT_SOURCE_DIR}/halley)
set(HOTRELOAD 0 CACHE BOOL "Sets whether to hot-reload this project")
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${HALLEY_PATH}/cmake/")

include(HalleyProject)

set (SOURCES
     # sources here
     )

set (HEADERS
     # headers here
     )

halleyProject(project_name "${SOURCES}" "${HEADERS}" "" ${CMAKE_CURRENT_SOURCE_DIR}/bin)