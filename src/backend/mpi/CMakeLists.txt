# Copyright (C) Eta Scale AB. Licensed under the Eta Scale Open Source License. See the LICENSE file for details.

add_library(argobackend-mpi mpi.cpp swdsm.cpp)
target_link_libraries(argobackend-mpi rt)

install(TARGETS argobackend-mpi
	COMPONENT "Runtime"
	RUNTIME DESTINATION bin
	LIBRARY DESTINATION lib
	ARCHIVE DESTINATION lib)
