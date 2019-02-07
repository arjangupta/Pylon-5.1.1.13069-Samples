
add_executable( grab_using_buffer_factory
    Grab_UsingBufferFactory.cpp
)

target_include_directories( grab_using_buffer_factory
    PUBLIC ${PYLON_INCLUDE_DIRS}
)

target_link_libraries( grab_using_buffer_factory
    ${PYLON}
)