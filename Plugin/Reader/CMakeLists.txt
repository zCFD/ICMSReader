set(classes
	vtkICMSReader)

set(private_headers "")

#vtk_module_find_package(
#  PACKAGE Gmsh
#  VERSION 4.1.0)

vtk_module_add_module(ICMSReader::vtkICMSReader
  CLASSES ${classes}
  PRIVATE_HEADERS ${private_headers})
vtk_module_link(ICMSReader::vtkICMSReader)

paraview_add_server_manager_xmls(
	XMLS  ICMSReader.xml)
