cmake_minimum_required(VERSION 2.8.12)
project(MD5Encrypter)

find_package(Poco CONFIG REQUIRED)

add_executable(md5 md5.cpp)
target_link_libraries(md5 Poco::Poco)

install(TARGETS md5
    RUNTIME DESTINATION bin
    ARCHIVE DESTINATION lib
    LIBRARY DESTINATION lib)

