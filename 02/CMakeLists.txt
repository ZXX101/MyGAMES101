set(TARGET_NAME 02)

find_package(Eigen3 CONFIG REQUIRED)
find_package(OpenCV  REQUIRED)

add_executable(${TARGET_NAME} main.cpp rasterizer.hpp rasterizer.cpp global.hpp Triangle.hpp Triangle.cpp)
target_link_libraries(${TARGET_NAME} PRIVATE ${OpenCV_LIBS} Eigen3::Eigen)