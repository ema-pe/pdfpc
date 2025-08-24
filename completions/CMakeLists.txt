if(NOT (WIN32 OR APPLE)) # Skip Windows and macOS for now.
    install(
        FILES pdfpc.bash
        DESTINATION "${CMAKE_INSTALL_PREFIX}/share/bash-completion/completions"
        PERMISSIONS OWNER_READ OWNER_WRITE GROUP_READ WORLD_READ
    )
endif()
