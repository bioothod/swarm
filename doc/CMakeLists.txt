CMAKE_MINIMUM_REQUIRED( VERSION 2.6 )
PROJECT( SWARM_DOC )

SET( SWARM_DOC_LANG English CACHE STRING "Documentation language")
SET( SWARM_DOC_BRIEF_MEMBER_DESC NO CACHE STRING "Include brief member descriptions after the members that are listed in the file and class documentation" )
SET( SWARM_DOC_EXTRACT_PRIVATE NO CACHE STRING "" )
SET( SWARM_DOC_EXTRACT_STATIC NO CACHE STRING "" )
SET( SWARM_DOC_QUIET NO CACHE STRING "Quiet documentation generation" )
SET( SWARM_DOC_FILE_PATTERNS "*.h *.hpp" CACHE STRING "Space separated wildcard patterns" )
SET( SWARM_DOC_EXCLUDE_PATTERNS "*_p.h *_p.hpp" CACHE STRING "Space separated wildcard patterns" )
SET( SWARM_DOC_EXCLUDE_SYMBOLS d_ptr CACHE STRING "Space separated wildcard patterns" )
SET( SWARM_DOC_SOURCE_BROWSER NO CACHE STRING "" )
SET( SWARM_DOC_INLINE_SOURCES NO CACHE STRING "" )
SET( SWARM_DOC_REFERENCED_BY_RELATION NO CACHE STRING "For each documented function all documented functions referencing it will be listed" )
SET( SWARM_DOC_REFERENCES_RELATION NO CACHE STRING "For each documented function all documented entities called/used by that function will be listed" )
SET( SWARM_DOC_GENERATE_ECLIPSEHELP NO CACHE STRING "" )
SET( SWARM_DOC_GENERATE_TREEVIEW YES CACHE STRING "" )
SET( SWARM_DOC_TREEVIEW_WIDTH 250 CACHE STRING "Set width if GENERATE_TREEVIEW is YES" )
SET( SWARM_DOC_EXPAND_ONLY_PREDEF NO CACHE STRING "" )
SET( SWARM_DOC_PREDEFINED Q_QDOC CACHE STRING "Predefined preprocessor macros names (like gcc -D ...)" )
SET( SWARM_DOC_CLASS_DIAGRAMS YES CACHE STRING "" )
SET( SWARM_DOC_HIDE_UNDOC_RELATIONS YES CACHE STRING "" )
SET( SWARM_DOC_HAVE_DOT NO CACHE STRING "Advanced graph visualization" )
SET( SWARM_DOC_UML_LOOK NO CACHE STRING "" )
SET( SWARM_DOC_CALL_GRAPH NO CACHE STRING "Works only if HAVE_DOT is YES. Enable only if you know what you are doing!" )
SET( SWARM_DOC_CALLER_GRAPH NO CACHE STRING "Works only if HAVE_DOT is YES. Enable only if you know what you are doing!" )
SET( SWARM_DOC_DOT_GRAPH_MAX_NODES 50 CACHE STRING "" )
SET( SWARM_DOC_MAX_DOT_GRAPH_DEPTH 0 CACHE STRING "0 is equal to no restriction" )

IF ( SWARM_DOC_SOURCE_BROWSER STREQUAL YES )
   SET (SWARM_DOC_LAYOUT_TAB_GUARD_GL_OP "")
   SET (SWARM_DOC_LAYOUT_TAB_GUARD_GL_ED "")
ELSE ()
   SET (SWARM_DOC_LAYOUT_TAB_GUARD_GL_OP "<!--")
   SET (SWARM_DOC_LAYOUT_TAB_GUARD_GL_ED "-->")
ENDIF ()

MARK_AS_ADVANCED(
   SWARM_DOC_BRIEF_MEMBER_DESC
   SWARM_DOC_EXTRACT_PRIVATE
   SWARM_DOC_EXTRACT_STATIC
   SWARM_DOC_QUIET
   SWARM_DOC_FILE_PATTERNS
   SWARM_DOC_EXCLUDE_PATTERNS
   SWARM_DOC_EXCLUDE_SYMBOLS
   SWARM_DOC_INLINE_SOURCES
   SWARM_DOC_REFERENCED_BY_RELATION
   SWARM_DOC_REFERENCES_RELATION
   SWARM_DOC_TREEVIEW_WIDTH
   SWARM_DOC_EXPAND_ONLY_PREDEF
   SWARM_DOC_PREDEFINED
   SWARM_DOC_HIDE_UNDOC_RELATIONS
   SWARM_DOC_CALL_GRAPH
   SWARM_DOC_CALLER_GRAPH
   SWARM_DOC_DOT_GRAPH_MAX_NODES
   SWARM_DOC_MAX_DOT_GRAPH_DEPTH
)
