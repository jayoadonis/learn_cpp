cmake_minimum_required(VERSION 3.16)
project("learn_cpp"
  LANGUAGES "CXX")

string(STRIP "${_ROOT_PROJECT_NAME}" _ROOT_PROJECT_NAME)
if(_ROOT_PROJECT_NAME)
  string(APPEND _ROOT_PROJECT_NAME ".${PROJECT_NAME}")
else()
  set(_ROOT_PROJECT_NAME "${PROJECT_NAME}")
endif()

add_subdirectory(project_structure)
add_subdirectory(object_oriented_programming)
add_subdirectory(algorithmic)
