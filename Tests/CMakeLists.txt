# helpers shared between all tests
add_subdirectory(CommonHelpers)

set(CMAKE_CXX_FLAGS " ${CMAKE_CXX_FLAGS} --coverage")

add_subdirectory_if(Benchmarks ACTS_BUILD_BENCHMARKS)
add_subdirectory_if(IntegrationTests ACTS_BUILD_INTEGRATIONTESTS)
add_subdirectory_if(UnitTests ACTS_BUILD_UNITTESTS)
