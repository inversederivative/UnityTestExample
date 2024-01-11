add_executable(UnityTest 
	Unity_tests.c

)


add_library(unity STATIC IMPORTED)
set_property(TARGET unity PROPERTY IMPORTED_LOCATION ${CMAKE_SOURCE_DIR}/library/Unity/libunity.a)

target_link_libraries(UnityTest unity)
