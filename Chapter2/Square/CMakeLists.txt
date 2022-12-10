add_executable(square square.cpp)
target_link_libraries(square "-framework OpenGL -framework GLUT")
target_link_libraries(square GLEW glfw soil2-debug glut)

