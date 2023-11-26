
include("${VTK_USE_FILE}")

add_executable(tutorial_step_4
    tutorial_step_4.cpp        
)

target_link_libraries(tutorial_step_4
    PRIVATE
        ${VTK_LIBRARIES}
)

vtk_module_autoinit(
    TARGETS 
        tutorial_step_4
    MODULES 
        ${VTK_LIBRARIES}
)
