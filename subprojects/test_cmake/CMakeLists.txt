add_custom_command(OUTPUT ${CMAKE_CURRENT_BINARY_DIR}/test.txt
	COMMAND cp -f ${CMAKE_SOURCE_DIR}/test.txt ${CMAKE_CURRENT_BINARY_DIR}/test.txt
	DEPENDS ${CMAKE_SOURCE_DIR}/test.txt)
add_custom_target(test_cp ALL DEPENDS ${CMAKE_CURRENT_BINARY_DIR}/test.txt)
