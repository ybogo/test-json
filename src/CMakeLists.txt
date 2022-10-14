project(main_executable)
file(GLOB SRC "*.cpp")

find_package(RapidJSON CONFIG REQUIRED)

add_executable(${PROJECT_NAME}_bin ${SRC})
target_link_libraries(${PROJECT_NAME}_bin PUBLIC rapidjson)