add_cast_component_internal(ExampleManagedComponent ExampleManagedComponent.hpp ExampleManagedComponent.cpp)

add_cast_component_internal(ExampleComponent ExampleComponent.hpp ExampleComponent.cpp)

add_cast_component_internal(SimpleServer SimpleServer.hpp SimpleServer.cpp)

add_cast_component_internal(SimpleAggregateServer SimpleAggregateServer.hpp SimpleAggregateServer.cpp)

add_cast_component_internal(WordServerClient WordServerClient.hpp WordServerClient.cpp)


include_directories(./comedyarch)
add_cast_component_internal(PriorityTester PriorityTester.hpp PriorityTester.cpp)
link_cast_component(PriorityTester ComedyShared)
