include_directories(.)

option(GOOGLE_PROFILER "use google profiler" NO)

# auto generated code
add_and_include_subdirectory (cast/slice)

# core code that is always used: basic components, data
add_and_include_subdirectory (cast/core)

# code that produces abstract classes for subarch components
add_and_include_subdirectory (cast/architecture)

# skeleton classes for testing
add_and_include_subdirectory (cast/examples)

# more in depth examples. 
add_and_include_subdirectory (cast/examples/comedyarch)

# server code for managing components at runtime
add_and_include_subdirectory (cast/server)

# tests, not ready for action yet
add_and_include_subdirectory (cast/testing)

# and these are the utility headers for users

set(headers cast/cast.hpp cast/core.hpp cast/architecture.hpp cast/server.hpp)

install(FILES ${headers} DESTINATION include/cast)
