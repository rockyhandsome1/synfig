add_library(mod_gradient MODULE "")

target_sources(mod_gradient
    PUBLIC
        "${CMAKE_CURRENT_LIST_DIR}/conicalgradient.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/radialgradient.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/main.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/curvegradient.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/lineargradient.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/spiralgradient.cpp"
)

install (
    TARGETS mod_gradient
    DESTINATION lib/synfig/modules
)
