cmake_minimum_required(VERSION 2.6.1)
project(Exo2)

find_package(Qt REQUIRED)
include(${QT_USE_FILE})

include_directories(/net/cremi/costerta/espaces/travail/GeLog/qcustomplot)
link_directories(/net/cremi/costerta/espaces/travail/GeLog/qcustomplot/sharedlib/compilation)


add_executable(CourbeCarre carre.cpp)
target_link_libraries(CourbeCarre ${QT_LIBRARIES} qcustomplot)

add_executable(GUISimple gui_simple.cpp)
target_link_libraries(GUISimple ${QT_LIBRARIES})
