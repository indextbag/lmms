set(CMAKE_C_FLAGS "")
set(CMAKE_CXX_FLAGS "")

IF(QT5 AND LMMS_BUILD_LINUX AND WANT_VST)
	set(BUILD_SHARED_LIBS OFF)
	add_subdirectory(qt5-x11embed)
ENDIF()

ADD_SUBDIRECTORY(rpmalloc)
