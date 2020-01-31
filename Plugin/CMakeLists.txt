paraview_add_plugin(ICMSReader
	  VERSION "1.0"
	  MODULES ICMSReader::vtkICMSReader
	  MODULE_FILES "${CMAKE_CURRENT_SOURCE_DIR}/Reader/vtk.module")
