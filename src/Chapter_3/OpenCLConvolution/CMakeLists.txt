add_executable( OpenCLConvolutionChap3 Convolution.cpp )
target_link_libraries( OpenCLConvolutionChap3 ${OPENCL_LIBRARIES} )
configure_file(Convolution.cl ${CMAKE_CURRENT_BINARY_DIR}/Convolution.cl COPYONLY)
