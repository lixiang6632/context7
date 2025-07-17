```
def open_portal(portal_mode: Optional[Enums.PortalMode] = None, version: Optional[str] = None) -> Portal:
Description: Open a new TIA Portal instance
Version-string in format major.minor e.g. \"18.0\"

*Returns* &rarr; `Portal` TIA Portal instance

| Parameters | Type | Description |
| --- | --- | --- |
| portal_mode | Enums.PortalMode | With or without user-interface |
| version | str | Version string of TIA Portal to be used in format major.minor e.g. 18.0, (Latest installed TIA Portal version by default) |

Example usage

portal = siemens_tia_scripting.open_portal(portal_mode = siemens_tia_scripting.Enums.PortalMode.WithGraphicalUserInterface, version = "18.0")

```

```
def attach_portal(portal_mode: Optional[Enums.PortalMode] = None, version: Optional[str] = None) -> Portal:
Description: Attach to running TIA Portal instance
Version-string in format major.minor e.g. \"18.0\"

*Returns* &rarr; `Portal` TIA Portal instance

| Parameters | Type | Description |
| --- | --- | --- |
| portal_mode | Enums.PortalMode | With or without user-interface |
| version | str | Version string of TIA Portal to be used in format major.minor e.g. 18.0, (Latest installed TIA Portal version by default) |

Example usage

portal = siemens_tia_scripting.attach_portal(portal_mode = Enums.PortalMode.WithGraphicalUserInterface, version = "18.0")

```

```
def open_attach_project(project_file_path: str, portal_mode: Optional[Enums.PortalMode] = None) -> Project:
Description: Attach to running TIA Portal instance with already open project
Or opens the project with a new instance of fitting TIA Portal version

*Returns* &rarr; `Project` TIA Project instance

| Parameters | Type | Description |
| --- | --- | --- |
| project_file_path | str | Full path of the project file |
| portal_mode | Enums.PortalMode | With or without user-interface |

Example usage

project = siemens_tia_scripting.open_attach_project(project_file_path = "C:\\ws\\testproj\\testproj.ap17", portal_mode = siemens_tia_scripting.Enums.PortalMode.WithGraphicalUserInterface)

```

```
def get_installed_bundles() -> List[ProductBundle]:
Description: Get a list of installed TIA Portal bundles

*Returns* &rarr; `List[ProductBundle]` List of installed bundles

Example usage

product_bundles = siemens_tia_scripting.get_installed_bundles()

```

```
def get_installed_products() -> List[Product]:
Description: Get a list of installed TIA Portal products

*Returns* &rarr; `List[Product]` List of installed products

Example usage

products = siemens_tia_scripting.get_installed_products()

```

```
def get_name() -> str:
Description: Get the name of the Test Suite application test

*Return* &rarr; `str` Name of the application test

Example usage

name = app_test.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the Test Suite application test

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property of the Application Test |

Example usage

property_value = app_test.get_property(name = "Property")

```

```
def get_name() -> str:
Description: Get the name of the PLC object

*Returns* &rarr; `str` Name of the PLC object

Example usage

name = plc_object.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the PLC object

*Returns* &rarr; `str` Name of the PLC object

Example usage

name = plc_object.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def is_consistent() -> bool:
Description: Check if the force table is consistent

*Returns* &rarr; `bool` True if consistent

Example usage

value = force_table.is_consistent()

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the global library

*Returns* &rarr; `str` Name of the global library

Example usage

name = global_lib.get_name()

```

```
def get_author() -> str:
Description: Get author of the global library

*Returns* &rarr; `str` Name of the author

Example usage

author = global_lib.get_author()

```

```
def get_path() -> str:
Description: Get the path of the global library

*Returns* &rarr; `str` Full path of the library

Example usage

path = global_lib.get_path()

```

```
def get_library_type_folder() -> LibraryTypeFolder:
Description: Get the folder containing library types & library type folders

*Returns* &rarr; `LibraryTypeFolder` Library type folder

Example usage

library_type = global_lib.get_library_type_folder()

```

```
def is_modified() -> bool:
Description: Check if the global library was modified

*Returns* &rarr; `bool` State if library was modified

Example usage

state = global_lib.is_modified()

```

```
def is_read_only() -> bool:
Description: Check if the global library is readonly

*Returns* &rarr; `bool` State if global library is readonly

Example usage

state = global_lib.is_read_only()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the global library info

*Returns* &rarr; `str` Name of the global library info

Example usage

name = global_lib_info.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the HMI

*Returns* &rarr; `str` Name of the HMI

Example usage

hmi_name = hmi.get_name()

```

```
def compile_hardware() -> bool:
Description: Compile the hardware of the HMI

*Returns* &rarr; `bool` Result of the compile

Returns true if compile has errors, otherwise returns false

Example usage

result = hmi.compile_hardware()

```

```
def compile_software() -> bool:
Description: Compile the software of the HMI

*Returns* &rarr; `bool` Result of the compile

Returns true if compile has errors, otherwise returns false

Example usage

result = hmi.compile_software()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the library type

*Returns* &rarr; `str` Name of the type

Example usage

name = lib_type.get_name()

```

```
def get_author() -> str:
Description: Get the author of the library type

*Returns* &rarr; `str` Author of the type

Example usage

author = lib_type.get_author()

```

```
def get_guid() -> str:
Description: Get the guid of the library type

*Returns* &rarr; `str` Guid of the type

Example usage

guid = lib_type.get_guid()

```

```
def get_versions() -> List[LibraryTypeVersion]:
Description: Get the versions of the library type

*Returns* &rarr; `List[LibraryTypeVersion]` Versions of the type

Example usage

versions = lib_type.get_versions()

```

```
def find_version(version: str) -> LibraryTypeVersion:
Description: Find the version of the library type

*Returns* &rarr; `LibraryTypeVersion` Version des Bibliothekstyp

Example usage

typeversion = lib_type.find_version(version = "1.0.0")

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the folder

*Returns* &rarr; `str` Name of the folder

Example usage

name = lib_folder.get_name()

```

```
def get_folders() -> List[LibraryTypeFolder]:
Description: Get the library type folders

*Returns* &rarr; `List[LibraryTypeFolder]` List of folders

Example usage

folders = lib_folder.get_folders()

```

```
def get_types() -> List[LibraryType]:
Description: Get the library types of the folder

*Returns* &rarr; `List[LibraryType]` List of types

Example usage

types = lib_folder.get_types()

```

```
def find_library_type(library_type_name: str) -> LibraryType:
Description: Find the library type by name

*Returns* &rarr; `LibraryType` Library type

| Parameters | Type | Description |
| --- | --- | --- |
| library_type_name | str | Name of the library type |

Example usage

type = lib_folder.find_library_type(library_type_name = "MyType")

```

```
def find_folder(folder_name: str) -> LibraryTypeFolder:
Description: Find the library type folder from the subfolders

*Returns* &rarr; `LibraryTypeFolder` Library type folder

| Parameters | Type | Description |
| --- | --- | --- |
| folder_name | str | Name of the subfolder |

Example usage

folder = lib_folder.find_folder(folder_name = "MyFolder")

```

```
def get_author() -> str:
Description: Get the author of the library type version

*Returns* &rarr; `str` Author

Example usage

author = projectlib.get_author()

```

```
def get_guid() -> str:
Description: Get the GUID of the library type version

*Returns* &rarr; `str` GUID

Example usage

guid = lib_type_version.get_guid()

```

```
def get_version_number() -> str:
Description: Get the version number of the library type version

*Returns* &rarr; `str` version number

Example usage

version_number = lib_type_version.get_version_number()

```

```
def get_modified_date() -> str:
Description: Get the modification date of the library type version

*Returns* &rarr; `str` Modification date

Example usage

date = lib_type_version.get_modified_date()

```

```
def get_state() -> str:
Description: Get the state of the library type version

*Returns* &rarr; `str` State of the library type version

Example usage

state = lib_type_version.get_state()

```

```
def get_type_object() -> LibraryType:
Description: Get the type of the library type version

*Returns* &rarr; `LibraryType` Library type object

Example usage

lib_type = lib_type_version.get_type_object()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the Named value data type

*Returns* &rarr; `str` Name of the NVT

Example usage

name = nvt.get_name()

```

```
def get_namespace() -> str:
Description: Get the name of the Named value data type namespace

*Returns* &rarr; `str` Name of the namespace

Example usage

name = nvt.get_namespace()

```

```
def get_name() -> str:
Description: Get the name of the PLC

*Returns* &rarr; `str` Name of the PLC

Example usage

plc_name = plc.get_name()

```

```
def get_online_state() -> str:
Description: Get the current online state of the PLC

*Returns* &rarr; `str` Online state

Example usage

plc.get_online_state()

```

```
def go_online(mode: str, pci_interface: str, ip_address: str) -> str:
Description: Go online with the PLC

*Returns* &rarr; `str` Online status

| Parameters | Type | Description |
| --- | --- | --- |
| mode | str | Configuration mode |
| pci_interface | str | PC Interface name |
| ip_address | str | IP address |

Example usage

plc.go_online(mode = "PN/IE", pci_interface = "PLCSIM", ip_address = "192.168.0.10")

```

```
def download(mode: str, pci_interface: str, ip_address: str) -> str:
Description: Download the PLC

*Returns* &rarr; `str` Result of the download

| Parameters | Type | Description |
| --- | --- | --- |
| mode | str | Configuration mode |
| pci_interface | str | PC Interface name |
| ip_address | str | IP address |

Example usage

result = plc.download(mode = "PN/IE", pci_interface = "PLCSIM", ip_address = "192.168.0.10")

```

```
def download_to_memory_card(download_directory: str) -> str:
Description: Download the PLC-configuration to memory card

*Returns* &rarr; `str` Result of the download

| Parameters | Type | Description |
| --- | --- | --- |
| download_directory | str | Download directory |

Example usage

result = plc.download_to_memory_card(download_directory = "E:\\")

```

```
def get_plc_tag_tables() -> List[PlcTagTable]:
Description: Get the list of the PLC Tag Tables

*Returns* &rarr; `List[PlcTagTable]` List of the PLC Tag tables

| Parameters | Type | Description |
| --- | --- | --- |
| folder_path | str | The group path of the item |

Example usage

plc_tag_tables = plc.get_plc_tag_tables(folder_path = "group1/group2")

```

```
def update_module_description() -> bool:
Description: Update the module description of the PLC

*Returns* &rarr; `bool` Result state

Example usage

result = plc.update_module_description()

```

```
def compile_hardware() -> bool:
Description: Compile the hardware of the PLC

*Returns* &rarr; `bool` Result of the compile

Returns true if compile has errors, otherwise returns false

Example usage

result = plc.compile_hardware()

```

```
def compile_software() -> bool:
Description: Compile the software of the PLC

*Returns* &rarr; `bool` Result of the compile

Returns true if compile has errors, otherwise returns false

Example usage

result = plc.compile_software()

```

```
def compare_to_online() -> bool:
Description: Compare actual PLC state to the online state

*Returns* &rarr; `bool` Result of the compare

Returns false if folders are Identical, otherwise returns true

Example usage

result = plc.compare_to_online()

```

```
def get_program_blocks() -> List[ProgramBlock]:
Description: Get the list of program blocks

*Returns* &rarr; `List[ProgramBlock]` List of the program blocks

| Parameters | Type | Description |
| --- | --- | --- |
| folder_path | str | The group path of the item |

Example usage

blocks = plc.get_program_blocks(folder_path = "group1/group2")

```

```
def get_system_blocks() -> List[SystemBlock]:
Description: Get the list of system blocks

*Returns* &rarr; `List[SystemBlock]` List of the system blocks

Example usage

blocks = plc.get_system_blocks()

```

```
def get_user_data_types() -> List[UserDataType]:
Description: Get the list of PLC data types

*Returns* &rarr; `List[UserDataType]` List of the PLC data types

| Parameters | Type | Description |
| --- | --- | --- |
| folder_path | str | The group path of the item |

Example usage

udts = plc.get_user_data_types(folder_path = "group1/group2")

```

```
def get_external_sources() -> List[ExternalSource]:
Description: Get the list of external source files

*Returns* &rarr; `List[ExternalSource]` List of the external source files of the PLC

| Parameters | Type | Description |
| --- | --- | --- |
| folder_path | str | The group path of the item |

Example usage

ext_sources = plc.get_external_sources()

```

```
def get_force_tables() -> List[ForceTable]:
Description: Get the list of force tables

*Returns* &rarr; `List[ForceTable]` List of the force tables of the PLC

Example usage

tables = plc.get_force_tables()

```

```
def get_watch_tables() -> List[WatchTable]:
Description: Get the list of watch tables

*Returns* &rarr; `List[WatchTable]` List of the watch tables of the PLC

| Parameters | Type | Description |
| --- | --- | --- |
| folder_path | str | The group path of the item |

Example usage

tables = plc.get_watch_tables()

```

```
def get_technology_objects() -> List[TechnologyObject]:
Description: Get the list of technology objects

*Returns* &rarr; `List[TechnologyObject]` List of the technology objects of the PLC

| Parameters | Type | Description |
| --- | --- | --- |
| folder_path | str | The group path of the item |

Example usage

tos = plc.get_technology_objects()

```

```
def get_software_units() -> List[SoftwareUnit]:
Description: Get the list of software units

*Returns* &rarr; `List[SoftwareUnit]` List of the software units

Example usage

software_units = plc.get_software_units()

```

```
def get_safety_administration() -> SafetyAdministration:
Description: Get Safety administration of the PLC

*Returns* &rarr; `SafetyAdministration` Safety Administration of the PLC

Example usage

sa = plc.get_safety_administration()

```

```
def safety_print(print_file: str) -> bool:
Description: Create a safety printout of the PLC and print it to a file

If the file already exists, it is overwritten.

*Returns* &rarr; `bool` Returns true on success

| Parameters | Type | Description |
| --- | --- | --- |
| print_file | str | Full path of the printout file |

Example usage

plc.safety_print(print_file = "C:\\ws\\safetyprint\\F_PLC_Printout.pdf")

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the PLC object

*Returns* &rarr; `str` Name of the PLC object

Example usage

name = plc_object.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the PLC object

*Returns* &rarr; `str` Name of the PLC object

Example usage

name = plc_object.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_plc_tags() -> List[PlcTag]:
Description: Get the list of PLC tags

*Returns* &rarr; `List[PlcTag]` List of the PLC tags

Example usage

plctags = table.get_plc_tags()

```

```
def get_user_constants() -> List[UserConstant]:
Description: Get the list of the user constants

*Returns* &rarr; `List[UserConstant]` List of the PLC constants

Example usage

constants = table.get_user_constants()

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_process_id() -> int:
Description: Get the TIA Portal process ID

*Returns* &rarr; `int` TIA Portal process id

Example usage

id = portal.get_process_id()

```

```
def open_project(project_file_path: str, server_project_view: Optional[bool] = None ) -> Project:
Description: Open a TIA Portal project or local session - optional in server view

*Returns* &rarr; `Project` TIA Portal project

| Parameters | Type | Description |
| --- | --- | --- |
| project_file_path | str | Full path of the project file |
| server_project_view | str | Default: false. If parameter set to true, open in server project view |

Example usage

project = portal.open_project(project_file_path = "C:\\ws\\testproj\\testproj.ap17")

```

```
def open_project_with_copy(project_file_path: str, target_directory_path: str, delete_existing_project: bool) -> Project:
Description: Open a TIA Portal project or local session in separate folder

*Returns* &rarr; `Project` TIA Portal project

| Parameters | Type | Description |
| --- | --- | --- |
| project_file_path | str | Full path of the project file |
| target_directory_path | str | Temporary path where the project should be copied before opened |
| delete_existing_project | bool | Defines if the temporary project should be deleted |

Example usage

project = portal.open_project_with_copy(project_file_path = "C:\\ws\\testproj\\testproj.ap17", target_directory_path = "C:\\ws\\temp" , delete_existing_project = True)

```

```
def retrieve_archive(target_directory_path: str, archive_file_path: str, delete_existing_project: bool) -> Project:
Description: Retrieve a TIA Portal project archive

*Returns* &rarr; `Project` TIA Portal project

| Parameters | Type | Description |
| --- | --- | --- |
| target_directory_path | str | Temporary path where project should be copied before opened |
| archive_file_path | str | Full path of the archived project file |
| delete_existing_project | bool | Defines if the temporary project should be deleted |

Example usage

project = portal.retrieve_archive(archive_file_path = "C:\\ws\\testproj\\testproj.zap17", target_directory_path = "C:\\ws\\temp" , delete_existing_project = True)

```

```
def create_project(target_directory_path: str, project_name: str, delete_existing_project: bool) -> Project:
Description: Create a new TIA Portal project

*Returns* &rarr; `Project` TIA Portal project

| Parameters | Type | Description |
| --- | --- | --- |
| target_directory_path | str | Temporary path where project should be copied before opened |
| project_name | str | Name of the new project |
| delete_existing_project | bool | Defines if the temporary project should be deleted |

Example usage

project = portal.create_project(target_directory_path = "C:\\ws\\temp" , project_name = "MyNewProject" delete_existing_project = True)

```

```
def get_project() -> Project:
Description: Get opened TIA Portal project of the current TIA Portal instance

*Returns* &rarr; `Project` TIA Portal project

Example usage

project = portal.get_project()

```

```
def get_global_library(library_name: str) -> GlobalLibrary:
Description: Get global library by name

*Returns* &rarr; `GlobalLibrary` Global Library

| Parameters | Type | Description |
| --- | --- | --- |
| library_name | str | Name of the global library |

Example usage

global_lib = portal.get_global_library(library_name = "GlobalLib1")

```

```
def open_global_library(library_path: str) -> GlobalLibrary:
Description: Open global library by path

*Returns* &rarr; `GlobalLibrary` Global Library

| Parameters | Type | Description |
| --- | --- | --- |
| library_path | str | Full path of the global library |

Example usage

global_lib = portal.open_global_library(library_path = "C:\\ws\\testlib\\testlib.al17")

```

```
def open_global_library_with_copy(target_directory_path: str, library_path: str, delete_existing_project: bool) -> GlobalLibrary:
Description: Open global library from a copy

*Returns* &rarr; `GlobalLibrary` Global Library

| Parameters | Type | Description |
| --- | --- | --- |
| target_directory_path | str | Temporary path where the library should be copied before opened |
| library_path | str | Full path of the global library |
| delete_existing_project | bool | Defines if the temporary project should be deleted |

Example usage

global_lib = portal.open_global_library_with_copy(target_directory_path = "C:\\ws\\temp", library_path = "C:\\ws\\testlib\\testlib.al17", delete_existing_project = True)

```

```
def retrieve_archive_library(target_directory_path: str, archive_file_path: str, delete_existing_project: bool) -> GlobalLibrary:
Description: Retrieve a TIA Portal library archive

*Returns* &rarr; `GlobalLibrary` Global Library

| Parameters | Type | Description |
| --- | --- | --- |
| target_directory_path | str | Temporary path where library should be copied before opened |
| archive_file_path | str | Full path of the archived library file |
| delete_existing_project | bool | Defines if the temporary project should be deleted |

Example usage

global_lib = portal.retrieve_archive_library(target_directory_path = "C:\\ws\\temp", archive_file_path = "C:\\ws\\testproj\\testlib.zal17", delete_existing_project = True)

```

```
def get_project_servers() -> List[ProjectServer]:
Description: Get a list of TIA Project-Servers found by host-filter

*Returns* &rarr; `List[ProjectServer]` List of TIA Project-Servers

| Parameters | Type | Description |
| --- | --- | --- |
| host_filter | str | Host of the TIA Project-Servers |

Example usage

portal.get_project_servers(host_filter = "CompanyServer")

```

```
def get_project_server(url: str) -> ProjectServer:
Description: Get the TIA Project-Server found by URL

*Returns* &rarr; `ProjectServer` TIA Project-Server

| Parameters | Type | Description |
| --- | --- | --- |
| url | str | URL of the TIA Project-Server |

Example usage

portal.get_project_server(url = "https://project.server.net:8735/")

```

```
def get_name() -> str:
Description: Get the name of the TIA Portal product

*Returns* &rarr; `str` Name of the TIA Portal product

Example usage

product_name = product.get_name()

```

```
def get_release() -> str:
Description: Get the release of the TIA Portal product

*Returns* &rarr; `str` Release tag of the TIA Portal product

Example usage

product_release = product.get_release()

```

```
def get_version() -> str:
Description: Get the version of the TIA Portal product

*Returns* &rarr; `str` Version of the TIA Portal product

Example usage

product_version = product.get_version()

```

```
def get_title() -> str:
Description: Get the title of the TIA Portal Bundle

*Returns* &rarr; `str` Title of the Siemens bundle

Example usage

bundle_title = bundle.get_title()

```

```
def get_release() -> str:
Description: Get the release of the TIA Portal Bundle

*Returns* &rarr; `str` Release of the Siemens bundle

Example usage

bundle_release = bundle.get_release()

```

```
def get_products() -> List[Product]:
Description: Get the list of products of the TIA Portal Bundle

*Returns* &rarr; `List[Product]` List of Siemens products

Example usage

bundle_products = bundle.get_products()

```

```
def get_name() -> str:
Description: Get the name of the PLC object

*Returns* &rarr; `str` Name of the PLC object

Example usage

name = plc_object.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def is_consistent() -> bool:
Description: Check if the program block is consistent

*Returns* &rarr; `bool` True if consistent

Example usage

value = programblock.is_consistent()

```

```
def get_type_version_guid() -> str:
Description: Get the GUID of the type version

*Returns* &rarr; `str` GUID

Example usage

guid = plc_object.get_type_version_guid()

```

```
def get_type_guid() -> str:
Description: Get the GUID of the type

*Returns* &rarr; `str` GUID

Example usage

guid = plc_object.get_type_guid()

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_portal() -> Portal:
Description: Get the TIA Portal instance from the current project

Example usage

portal = project.get_portal()

```

```
def archive(target_directory_path: str, archive_name: str, delete_existing_archive: bool) -> str:
Description: Archive the TIA Portal project

*Returns* &rarr; `str` Full path of the new archive

| Parameters | Type | Description |
| --- | --- | --- |
| target_directory_path | str | Folder path where archive should be placed |
| archive_name | str | name of the archive file |
| delete_existing_archive | bool | Set if the output file should be deleted first |

Example usage

archive_fullpath = project.archive(target_directory_path = "C:\\ws\\newfolder", archive_name = "testproj" , delete_existing_archive = True)

```

```
def save_as(target_directory_path: str, project_name: str) -> str:
Description: Save the TIA Portal project under another path and name

*Returns* &rarr; `str` Full path of the saved project

| Parameters | Type | Description |
| --- | --- | --- |
| target_directory_path | str | Folder path where project should be saved |
| project_name | str | Name of the project name |

Example usage

project_file_path = project.save_as(target_directory_path = "C:\\ws\\newfolder", project_name = "testproj")

```

```
def export_cax_data(export_file_path: str, log_file_path: str) -> bool:
Description: Export the CAx data of the TIA Portal project

*Returns* &rarr; `bool` Result state of the export

| Parameters | Type | Description |
| --- | --- | --- |
| export_file_path | str | Full path of the export file |
| log_file_path | str | Full path of the log file |

Example usage

result = project.export_cax_data(export_file_path = "C:\\ws\\exportfolder\\exportCAX.aml", log_file_path = "C:\\ws\\exportfolder\\exportCAX.log")

```

```
def import_cax_data(import_file_path: str, log_file_path: str) -> bool:
Description: Import CAx data to the TIA Portal project

*Returns* &rarr; `bool` Result state of the import

| Parameters | Type | Description |
| --- | --- | --- |
| import_file_path | str | Fullpath of the import file |
| log_file_path | str | Fullpath of the log file |

Example usage

result = project.import_cax_data(import_file_path = "C:\\ws\\importfolder\\importCAX.aml", log_file_path = "C:\\ws\\importfolder\\importCAX.log")

```

```
def get_plcs() -> List[Plc]:
Description: Get a list of PLCs in the TIA Portal project

*Returns* &rarr; `List[Plc]` All PLC's as list

Example usage

plcs = project.get_plcs()
for plc in plcs:
...

```

```
def get_hmis() -> List[Hmi]:
Description: Get a list of HMIs in the TIA Portal project

*Returns* &rarr; `List[Hmi]` All HMI's as list

Example usage

hmis = project.get_hmis()
for hmi in hmis:
...

```

```
def get_application_tests() -> List[ApplicationTest]:
Description: Get a list of Test Suite application tests in the TIA Portal project

Needs Test Suite installed and licensed.

*Returns* &rarr; `List[ApplicationTest]` All Application tests as list

Example usage

tests = project.get_application_tests()

```

```
def get_system_tests() -> List[SystemTest]:
Description: Get a list of Test Suite system tests in the TIA Portal project

Needs Test Suite installed and licensed.

*Returns* &rarr; `List[SystemTest]` All System tests as list

Example usage

tests = project.get_system_tests()

```

```
def get_rule_sets() -> List[RuleSet]:
Description: Get a list of Test Suite Styleguide rule sets in the TIA Portal project

Needs Test Suite installed and licensed.

*Returns* &rarr; `List[RuleSet]` All Rule sets as list

Example usage

rule_sets = project.get_rule_sets()

```

```
def get_project_library() -> ProjectLibrary:
Description: Get the project library

*Returns* &rarr; `ProjectLibrary` Project library

Example usage

project_lib = project.get_project_library()

```

```
def import_umac_config(import_file_path: str) -> int:
Description: Import UMAC and UMC Configuration to the TIA Portal project

| Parameters | Type | Description |
| --- | --- | --- |
| import_file_path | str | Full path of the import file |
| secret | str | Secret for the encryption (optional if passwords encrypted) |
| secret_env_name | str | Name of the environment variable where Secret is stored (optional if passwords encrypted) |

Example usage

project.import_umac_config(import_file_path = "C:\\ws\\importfolder\\importUMAC.json", secret_env_name = "MYSECRETENV")

```

```
def encrypt_umac_config(umac_file_path: str, secret: str, secret_env_name: str) -> str:
Description: Encrypt UMAC and UMC configuration from the TIA Portal project with provided secret

| Parameters | Type | Description |
| --- | --- | --- |
| umac_file_path | str | Full path of the umac config file |
| secret | str | Secret for the encryption |
| secret_env_name | str | Name of the environment variable where secret value is stored |

Example usage

project.encrypt_umac_config(umac_file_path = "C:\\ws\\exportfolder\\exportUMAC.json", secret = "mySecret")

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_type_folder() -> LibraryTypeFolder:
Description: Get the folder containing library types & library type folders

*Returns* &rarr; `LibraryTypeFolder` Library type folder

Example usage

typefolder = projectlib.get_type_folder()

```

```
def get_host() -> str:
Description: Get the host of the TIA Project-Server

*Returns* &rarr; `str` Host

Example usage

host = server_project.get_host()

```

```
def get_port() -> int:
Description: Get the port of the TIA Project-Server

*Returns* &rarr; `int` Port number

Example usage

port = server_project.get_port()

```

```
def get_server_name() -> str:
Description: Get the server name of the TIA Project-Server

*Returns* &rarr; `str` Server name

Example usage

name = server_project.get_server_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the Test Suite style guide rule set

*Return* &rarr; `str` Name of the rule set

Example usage

name = rule.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the Test Suite style guide rule set

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property of the rule set |

Example usage

property_value = rule.get_property(name = "Property")

```

```
def is_logged_on() -> bool:
Description: Check if user is logged in to Safety administration offline program

*Returns* &rarr; `bool` Status of login

Example usage

status = safety_admin.is_logged_on()

```

```
def is_password_set() -> bool:
Description: Check if the safety administration has a password set for the safety offline program

*Returns* &rarr; `bool` Status if password is set

Example usage

status = safety_admin.is_password_set()

```

```
def get_offline_serial_number() -> str:
Description: Get the offline serial number

*Returns* &rarr; `str` Offline serial number

Example usage

value = safety_admin.get_offline_serial_number()

```

```
def get_name() -> str:
Description: Get the name of the software unit

*Return* &rarr; `str` Name of the software unit
*

Example usage

name = software_unit.get_name()

```

```
def get_plc_tag_tables() -> List[PlcTagTable]:
Description: Get the list of the PLC tag tables

*Returns* &rarr; `List[PlcTagTable]` List of the PLC tag tables of the software unit

Example usage

pcl_tag_tables = software_unit.get_plc_tag_tables()

```

```
def get_program_blocks() -> List[ProgramBlock]:
Description: Get the list of the program blocks

*Returns* &rarr; `List[ProgramBlock]` List of the program blocks of the software unit

Example usage

blocks = software_unit.get_program_blocks()

```

```
def get_system_blocks() -> List[SystemBlock]:
Description: Get the list of the system blocks

*Returns* &rarr; `List[SystemBlock]` List of the system blocks of the software unit

Example usage

blocks = software_unit.get_system_blocks()

```

```
def get_user_data_types() -> List[UserDataType]:
Description: Get the list of the user data types

*Returns* &rarr; `List[UserDataType]` List of the user data types of the software unit

Example usage

udts = software_unit.get_user_data_types()

```

```
def get_external_sources() -> List[ExternalSource]:
Description: Get the list of the external sources

*Returns* &rarr; `List[ExternalSource]` List of the external sources of the software unit

Example usage

ext_sources = software_unit.get_external_sources()

```

```
def get_named_value_types() -> List[NamedValueType]:
Description: Get the list of the named value types

*Returns* &rarr; `List[NamedValueType]` List of the named value types of the software unit

Example usage

nvts = software_unit.get_named_value_types()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the PLC object

*Returns* &rarr; `str` Name of the PLC object

Example usage

name = plc_object.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def is_consistent() -> bool:
Description: Check if the system block is consistent

*Returns* &rarr; `bool` True if consistent

Example usage

value = systemblock.is_consistent()

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the Test Suite system test

*Returns* &rarr; `str` Name of the system test

Example usage

name = sys_test.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the PLC object

*Returns* &rarr; `str` Name of the PLC object

Example usage

name = plc_object.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def is_consistent() -> bool:
Description: Check if the technology object is consistent

*Returns* &rarr; `bool` True if consistent

Example usage

value = to.is_consistent()

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the PLC object

*Returns* &rarr; `str` Name of the PLC object

Example usage

name = plc_object.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the PLC object

*Returns* &rarr; `str` Name of the PLC object

Example usage

name = plc_object.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def is_consistent() -> bool:
Description: Check if the PLC data type is consistent

*Returns* &rarr; `bool` True if consistent

Example usage

value = udt.is_consistent()

```

```
def get_type_version_guid() -> str:
Description: Get the GUID of the type version

*Returns* &rarr; `str` GUID

Example usage

guid = plc_object.get_type_version_guid()

```

```
def get_type_guid() -> str:
Description: Get the GUID of the type

*Returns* &rarr; `str` GUID

Example usage

guid = plc_object.get_type_guid()

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

```
def get_name() -> str:
Description: Get the name of the PLC object

*Returns* &rarr; `str` Name of the PLC object

Example usage

name = plc_object.get_name()

```

```
def get_property(name: str) -> str:
Description: Get the property of the object

Properties which are not string will be converted to string if possible.

*Returns* &rarr; `str` Value of the property as string

| Parameters | Type | Description |
| --- | --- | --- |
| name | str | Property name of the object |

Example usage

property_value = tiap_object.get_property(name = "CreationDate")

```

```
def is_consistent() -> bool:
Description: Check if the watch table is consistent

*Returns* &rarr; `bool` True if consistent

Example usage

value = watch_table.is_consistent()

```

```
def get_properties() -> List[str]:
Description: Get all properties of the object

*Returns* &rarr; `List[str]` Names of the attributes

Example usage

properties = tiap_object.get_properties()

```

