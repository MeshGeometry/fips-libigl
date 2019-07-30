if (NOT FIPS_IMPORT)
    cmake_minimum_required(VERSION 2.8)
    get_filename_component(FIPS_ROOT_DIR "../fips" ABSOLUTE)
    include("${FIPS_ROOT_DIR}/cmake/fips.cmake")
    fips_setup()
    fips_project(fips-libigl)
endif()

set(FIPS_EXCEPTIONS ON CACHE BOOL "Enable C++ exceptions" FORCE)
set(FIPS_RTTI  ON CACHE BOOL "Enable C++ RTTI" FORCE)

if ((FIPS_MACOS OR FIPS_WINDOWS OR FIPS_LINUX) AND NOT (FIPS_RASPBERRYPI OR FIPS_OSX_USE_ARC OR FIPS_UWP))



endif()
