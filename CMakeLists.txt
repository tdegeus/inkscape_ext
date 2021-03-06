# required to specify the c++ standard
cmake_minimum_required(VERSION 3.0)

# define project information
project(GooseSLURM)

# option: install all
option(ALL "Install all binaries" OFF)

# initialize list with binaries
set(PROJECT_BINARIES
  "svg2pdf"
  "svg2png"
  "svgfit"
  "svglayerswitch"
)

# install binaries
INSTALL(PROGRAMS ${CMAKE_CURRENT_SOURCE_DIR}/${PROJECT_BINARIES} DESTINATION bin)

# print information to screen
message(STATUS "")
message(STATUS "+-------------------------------------------------------------------------------")
message(STATUS "|")
message(STATUS "| Install:")
message(STATUS "|")
message(STATUS "|   ${PROJECT_BINARIES}")
message(STATUS "|")
message(STATUS "| Use 'make install' to install in:")
message(STATUS "|")
message(STATUS "|   ${CMAKE_INSTALL_PREFIX}")
message(STATUS "|")
message(STATUS "| To specify a custom directory, add the following cmake-option:")
message(STATUS "|")
message(STATUS "|   cmake ... -DCMAKE_INSTALL_PREFIX=yourprefix")
message(STATUS "|")
message(STATUS "| For custom paths, add the following line to your '~/.bashrc'")
message(STATUS "|")
message(STATUS "|   export PATH=${CMAKE_INSTALL_PREFIX}/bin:$PATH")
message(STATUS "|")
message(STATUS "+-------------------------------------------------------------------------------")
message(STATUS "")
