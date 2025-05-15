FIND_PACKAGE(GLUT REQUIRED)
FIND_PACKAGE(OpenGL REQUIRED)
FIND_PACKAGE(GLEW REQUIRED)

add_executable( sinewave sinewave.cpp )
target_link_libraries( sinewave ${OPENCL_LIBRARIES} ${GLUT_LIBRARIES} ${GLEW_LIBRARY} ${OPENGL_LIBRARY})

configure_file(sinewave.cl ${CMAKE_CURRENT_BINARY_DIR}/sinewave.cl COPYONLY)
