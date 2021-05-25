find_package(Catch2 REQUIRED)

add_executable(unit_tests
  main.cpp	
  polynomial.cpp
  )


target_link_libraries(unit_tests
  PUBLIC
    Catch2::Catch2
  )

include(Catch)
catch_discover_tests(unit_tests)
