ENABLE_TESTING()

set(tlsunittest_bin_SRCS tlsunittest.cpp)  

add_executable(tlsunittest ${tlsunittest_bin_SRCS} )

target_link_qca_test_libraries(tlsunittest)

add_qca_test(tlsunittest "TransportLayerSecurity")
