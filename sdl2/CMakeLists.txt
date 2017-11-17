cmake_minimum_required ( VERSION 2.6 )
# Здесь имя нашего проекта.

set (PROJECT sdl2 ) 
 
project (${PROJECT})

# - имя исполняемого файла

set (SOURSE_FILES  main.cpp)

# заголовочные файлы, которые следует добавить 
# для компиляции проекта
include_directories ("C:/MinGW/include")
#include_directories ( /path/to/headers_2 )
# ...
# библиоеки, которые следует добавить 
# для линковки проекта
link_directories ("C:/MinGW/lib")
#link_directories ( /path/to/lib_2 )
# ...
add_executable ( ${PROJECT} ${SOURSE_FILES} )

# добавление имени библиотеки
# требуемой для линковки проекта
target_link_libraries( ${PROJECT} mingw32 SDL2main SDL2 )
#target_link_libraries( ${APP_NAME} name_2 )
# ...
