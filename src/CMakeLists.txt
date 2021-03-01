project(gali LANGUAGES C CXX)

set(GALI_MAIN_SOURCE_PATH ".")
set(GALI_MAIN_SOURCE

    "${GALI_MAIN_SOURCE_PATH}/main.cpp"

)

add_executable(${GALI_PROG_NAME} ${GALI_MAIN_SOURCE})