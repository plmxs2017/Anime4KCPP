project(Anime4KCPP_CLI LANGUAGES CXX)

if(Build_CLI)

    aux_source_directory(src SOURCE)

    include_directories(${TOP_DIR}/Anime4KCore/include)

    add_compile_definitions(COMPILER="${CMAKE_CXX_COMPILER_ID}")

    add_executable(${PROJECT_NAME} ${SOURCE})

    include(${TOP_DIR}/cmake/ThirdPartyForCLI.cmake)

endif()
