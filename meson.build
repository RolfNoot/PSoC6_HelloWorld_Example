project('PSoC6_dual_core', 'c', 'cpp',
    version : '0.1',
    default_options : ['c_std=c11', 'cpp_std=c++14', 'warning_level=3']
)

[host_machine]
system     = 'none'
cpu_family = 'arm'
cpu        = 'cortex-m4'
endian     = 'little'

#================================================================================================================================#
# check Creator_PostBuild version and set various variables for possible use

# Creator_PostBuild_Minumum_Version: '2.20' - used for checking Creator_PostBuild minimum version, do not remove

# Creator_PostBuild_Version_Line - automatic insert of Creator_PostBuild version. Do not edit the line below


# Creator_PostBuild_DateTime_Line - automatic insert of Creator Generated DateTime. Do not edit the line below


# Creator_PostBuild_devicePart_Line - automatic insert of device part by Creator_PostBuild. Do not edit the line below


# Creator_PostBuild_linkerFile_Line - automatic insert of linker file by Creator_PostBuild. Do not edit the line below


# Creator_PostBuild_SVDfile_Line - automatic insert of SVD file by Creator_PostBuild. Do not edit the line below


# Creator_PostBuild_prePostBuild_Lines - automatic insert of pre- and postbuild commands by Creator_PostBuild. Do not edit the two line below



# set directories
# Creator_PostBuild_Directory_Line - automatic insert of Creator Project main directory. Do not edit the line below


# OTX_Extension_print(PROJECTNAME = '${workspaceFolderBasename}')
PROJECTNAME = 'PSoC6_HelloWorld_Example'

# OTX_Extension_print(ONETHINX_PACK_LOC = '${env:ONETHINX_PACK_LOC}')
ONETHINX_PACK_LOC = '/Applications/OTX-Maestro'

CONFIG_DIR 			= ONETHINX_PACK_LOC + '/config'
GCC_DIR 			= ONETHINX_PACK_LOC + '/gcc-arm/bin'
BIN_DIR 			= ONETHINX_PACK_LOC + '/bin'
SCRIPTS_DIR 		= ONETHINX_PACK_LOC + '/config/scripts'

MESON_SOURCE_LOC 	= meson.current_source_dir()
CREATOR_DIR 		= MESON_SOURCE_LOC + '/' + creatorDirectory

#================================================================================================================================#
# import tools

objcopy  		= find_program(GCC_DIR + '/arm-none-eabi-objcopy').path()
objdump  		= find_program(GCC_DIR + '/arm-none-eabi-objdump').path()
size     		= find_program(GCC_DIR + '/arm-none-eabi-size').path()
gdb      		= find_program(GCC_DIR + '/arm-none-eabi-gdb').path()
cymcuelftool 	= find_program(BIN_DIR + '/cymcuelftool').path()
readelf  		= find_program(GCC_DIR + '/arm-none-eabi-readelf').path()
memcalc 		= find_program(BIN_DIR + '/memcalc').path()

# Custom targets for signing and merging
#private_key = dependencies_dir / 'keys/rsa_private.txt'

#================================================================================================================================#
# setup compile & link arguments

assembler_args_m0 = [
# Creator_PostBuild_AssemblerOptions_Start (ID:CortexM0p) - automatic insert of assembler options by Creator_PostBuild. Do not edit below this line
# Creator_PostBuild_AssemblerOptions_End - automatic insert of assembler options by Creator_PostBuild. Do not edit above this line
]

compiler_args_m0  = [
# Creator_PostBuild_CompilerOptions_Start (ID:CortexM0p) - automatic insert of compiler options by Creator_PostBuild. Do not edit below this line
# Creator_PostBuild_CompilerOptions_End - automatic insert of compiler options by Creator_PostBuild. Do not edit above this line
	'-O0'
]

linker_args_m0    = [
# Creator_PostBuild_LinkerOptions_Start (ID:CortexM0p) - automatic insert of linker options by Creator_PostBuild. Do not edit below this line
# Creator_PostBuild_LinkerOptions_End - automatic insert of linker options by Creator_PostBuild. Do not edit above this line
]

#================================================================================================================================#
# setup include folders and source files

include_dirs_m0   = [
# OTX_Extension_HeaderFiles_Start (folder:source/CortexM0)- automatic insert of source files by the OTX VSCode extension. Do not edit below this line
# OTX_Extension_HeaderFiles_End - automatic insert of source files by the OTX VSCode extension. Do not edit above this line
# Creator_PostBuild_IncludeFolders_Start (ID:CortexM0p) - automatic insert of include header folders by Creator_PostBuild. Do not edit below this line
# Creator_PostBuild_IncludeFolders_End - automatic insert of include header folders by Creator_PostBuild. Do not edit above this line
]


sourcefiles_m0    = [
	# manual insert of additional needed sources
	creatorDirectory + '/gcc/startup_psoc6_01_cm0plus.S',
	creatorDirectory + '/system_psoc6_cm0plus.c',
# OTX_Extension_SourceFiles_Start (folder:source/CortexM0) - automatic insert of source files by the OTX VSCode extension. Do not edit below this line
# OTX_Extension_SourceFiles_End - automatic insert of source files by the OTX VSCode extension. Do not edit above this line
# Creator_PostBuild_SourceFiles_Start (ID:CortexM0p) - automatic insert of source files by Creator_PostBuild. Do not edit below this line
# Creator_PostBuild_SourceFiles_End - automatic insert of source files by Creator_PostBuild. Do not edit above this line
]

#================================================================================================================================#
# include libraries

#cc = meson.get_compiler('c')

# example: include library.a from directory
#link_deps = declare_dependency( dependencies : cc.find_library('library', dirs : ['directory/libdir']) )
link_deps_m0 = [
# Creator_PostBuild_LibSources_Start (ID:CortexM0p) - automatic insert of include source files by Creator_PostBuild. Do not edit below this line
# Creator_PostBuild_LibSources_End - automatic insert of include source files by Creator_PostBuild. Do not edit above this line
]


#================================================================================================================================#
# setup compile & link arguments

assembler_args_m4 = [
# Creator_PostBuild_AssemblerOptions_Start (ID:CortexM4) - automatic insert of assembler options by Creator_PostBuild. Do not edit below this line
# Creator_PostBuild_AssemblerOptions_End - automatic insert of assembler options by Creator_PostBuild. Do not edit above this line
]

compiler_args_m4  = [
# Creator_PostBuild_CompilerOptions_Start (ID:CortexM4) - automatic insert of compiler options by Creator_PostBuild. Do not edit below this line
# Creator_PostBuild_CompilerOptions_End - automatic insert of compiler options by Creator_PostBuild. Do not edit above this line
	'-O0'
]

linker_args_m4    = [
# Creator_PostBuild_LinkerOptions_Start (ID:CortexM4) - automatic insert of linker options by Creator_PostBuild. Do not edit below this line
# Creator_PostBuild_LinkerOptions_End - automatic insert of linker options by Creator_PostBuild. Do not edit above this line
]

#================================================================================================================================#
# setup include folders and source files

include_dirs_m4   = [
# OTX_Extension_HeaderFiles_Start (folder:source/CortexM4) - automatic insert of source files by the OTX VSCode extension. Do not edit below this line
# OTX_Extension_HeaderFiles_End - automatic insert of source files by the OTX VSCode extension. Do not edit above this line
# Creator_PostBuild_IncludeFolders_Start (ID:CortexM4) - automatic insert of include header folders by Creator_PostBuild. Do not edit below this line
# Creator_PostBuild_IncludeFolders_End - automatic insert of include header folders by Creator_PostBuild. Do not edit above this line
]

sourcefiles_m4    = [
	# manual insert of additional needed sources
	creatorDirectory + '/gcc/startup_psoc6_01_cm4.S',
	creatorDirectory + '/system_psoc6_cm4.c',
# OTX_Extension_SourceFiles_Start (folder:source/CortexM4) - automatic insert of source files by the OTX VSCode extension. Do not edit below this line
# OTX_Extension_SourceFiles_End - automatic insert of source files by the OTX VSCode extension. Do not edit above this line
# Creator_PostBuild_SourceFiles_Start (ID:CortexM4) - automatic insert of source files by Creator_PostBuild. Do not edit below this line
# Creator_PostBuild_SourceFiles_End - automatic insert of source files by Creator_PostBuild. Do not edit above this line
]

#================================================================================================================================#
# include libraries

#cc = meson.get_compiler('c')

# example: include library.a from directory
#link_deps = declare_dependency( dependencies : cc.find_library('library', dirs : ['directory/libdir']) )
link_deps_m4 = [
# Creator_PostBuild_LibSources_Start (ID:CortexM4) - automatic insert of include source files by Creator_PostBuild. Do not edit below this line
# Creator_PostBuild_LibSources_End - automatic insert of include source files by Creator_PostBuild. Do not edit above this line
]

#================================================================================================================================#
# run prebuild script 

#prebuild = custom_target('prebuild', output : 'buildversion.h', command : [MESON_SOURCE_LOC+'/config/prebuild.bash']) #use prebuild.bash / prebuild.bat file
#link_deps += declare_dependency( sources : [prebuild])

#================================================================================================================================#
# build executables

main_m0 = executable(
            PROJECTNAME+'_M0',    [sourcefiles_m0],
            name_suffix         : 'elf',
            c_args              : [compiler_args_m0],
            link_args           : [linker_args_m0],
            dependencies        : link_deps_m0,
            include_directories : [include_dirs_m0]
)

main_m4 = executable(
            PROJECTNAME+'_M4',    [sourcefiles_m4],
            name_suffix         : 'elf',
            c_args              : [compiler_args_m4],
            link_args           : [linker_args_m4],
            dependencies        : link_deps_m4,
            include_directories : [include_dirs_m4]
)

# Custom targets for signing executables

main_m0_signed = custom_target( 'main_m0_signed',
  			input 				: main_m0,
  			output 				: PROJECTNAME+'_M0_signed.elf',
  			command 			: [ cymcuelftool, '--sign', '@INPUT@', '--output', '@OUTPUT@' ],
  			build_by_default : true
)

main_m4_signed = custom_target( 'main_m4_signed',
			input 				: main_m4,
			output 				: PROJECTNAME+'_M4_signed.elf',
			command 			: [ cymcuelftool, '--sign', '@INPUT@', '--output', '@OUTPUT@' ],
			build_by_default : true
)

# Custom targets for merging signed executables and hex file

merged_m0_debug = custom_target( 'merged_m0_debug',
			input 				: [main_m0_signed, main_m4_signed],
			output 				: [PROJECTNAME+'_M0_debug.elf', PROJECTNAME+'_merged.hex'],
			command 			: [ cymcuelftool, '--merge', '@INPUT0@', '@INPUT1@', '--output', '@OUTPUT0@', '--hex', '@OUTPUT1@', ],
			build_by_default : true
)
merged_m4_debug = custom_target( 'merged_m4_debug',
			input 				: [main_m4_signed, main_m0_signed],
			output 				: PROJECTNAME+'_M4_debug.elf',
			command 			: [ cymcuelftool, '--merge', '@INPUT0@', '@INPUT1@', '--output', '@OUTPUT@' ],
			build_by_default : true
)

# Custom targets for showing memory usage

showoutput = custom_target( 'showoutput',
			input 				: [main_m0, main_m4],
			depends				: [merged_m0_debug, merged_m4_debug],
			output           	: [PROJECTNAME + '.memcalc_m0.txt', PROJECTNAME + '.memcalc_m4.txt'],
			command             : [
        							[memcalc,'-Dual', '-InfoMemory Usage Map Cortex M0p:', readelf, '@INPUT0@', '0x080000', '0x24000', '0x10000000', '0x08000000', '@OUTPUT0@'],  #Flash 0x080000   SRAM 0x24000   Flash start 0x10000000   SRAM start 0x08000000
									['-InfoMemory Usage Map Cortex M4:', readelf, '@INPUT1@', '0x080000', '0x23800', '0x10080000', '0x08024000', '@OUTPUT1@']  #Flash 0x080000   SRAM 0x23800   Flash start 0x10080000   SRAM start 0x08024000
								],
			build_by_default 	: true,
			console			 	: true,
			build_always_stale  : true			# set to false to show memory usage only when sources have been changed
)
