add_wast_executable(TARGET hello
        INCLUDE_FOLDERS "${STANDARD_INCLUDE_FOLDERS}"
        LIBRARIES libc libc++ eosiolib
        DESTINATION_FOLDER ${CMAKE_CURRENT_BINARY_DIR}
        )
