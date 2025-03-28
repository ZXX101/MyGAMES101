set(TARGET_NAME 00)

find_package(Eigen3 CONFIG REQUIRED)
add_executable(${TARGET_NAME} main.cpp)
target_link_libraries(${TARGET_NAME} PRIVATE Eigen3::Eigen)