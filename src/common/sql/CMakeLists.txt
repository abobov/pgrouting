# Append in local scope
LIST(APPEND PACKAGE_SQL_FILES
    ${CMAKE_CURRENT_SOURCE_DIR}/pgRouting-header.sql
    ${CMAKE_CURRENT_SOURCE_DIR}/pgrouting-types.sql
    ${CMAKE_CURRENT_SOURCE_DIR}/pgrouting_version.sql
    ${CMAKE_CURRENT_SOURCE_DIR}/pgrouting_utilities.sql
    ${CMAKE_CURRENT_SOURCE_DIR}/pgr_parameter_check.sql
    ${CMAKE_CURRENT_SOURCE_DIR}/utilities_pgr.sql
    ${CMAKE_CURRENT_SOURCE_DIR}/noUnderUtilities.sql
    ${CMAKE_CURRENT_SOURCE_DIR}/createIndex.sql
    #${CMAKE_CURRENT_SOURCE_DIR}/findClosestEdge.sql
    ${CMAKE_CURRENT_SOURCE_DIR}/_point_toId.sql
    
)

# set in parent scope
SET(PACKAGE_SQL_FILES "${PACKAGE_SQL_FILES}" PARENT_SCOPE)
