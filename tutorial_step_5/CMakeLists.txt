
include("${VTK_USE_FILE}")

add_executable(tutorial_step_5
    tutorial_step_5.cpp        
)

target_link_libraries(tutorial_step_5
    PRIVATE
        ${VTK_LIBRARIES}
)

vtk_module_autoinit(
    TARGETS 
        tutorial_step_5
    MODULES 
        ${VTK_LIBRARIES}
)
