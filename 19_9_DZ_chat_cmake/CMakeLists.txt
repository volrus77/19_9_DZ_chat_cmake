# CMakeList.txt: проект CMake для 19_9_DZ_chat_cmake; включите исходный код и определения,
# укажите здесь логику для конкретного проекта.
#
cmake_minimum_required (VERSION 3.8)

# Добавьте источник в исполняемый файл этого проекта.
add_executable (19_9_DZ_chat_cmake "main.cpp" "chat.h" "chat.cpp" "Message.h" "AuthData.h" "sha1.h" "sha1.cpp")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET 19_9_DZ_chat_cmake PROPERTY CXX_STANDARD 20)
endif()

# TODO: Добавьте тесты и целевые объекты, если это необходимо.
