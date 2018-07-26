find_path( FEI_INCLUDE mfxfeihevc.h PATHS ${MFX_INCLUDE} )

include_directories (
  ${CMAKE_CURRENT_SOURCE_DIR}/../../samples/sample_common/include
  ${CMAKE_CURRENT_SOURCE_DIR}/include
)

list( APPEND LIBS_VARIANT sample_common )

make_executable( shortname universal "nosafestring" )
set( defs "" )
