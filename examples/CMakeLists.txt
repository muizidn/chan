function(add_example NAME)
    add_executable(${NAME} ${NAME}.c)
    target_link_libraries(${NAME} chan)
endfunction(add_example NAME)

add_example(buffered)
add_example(close)
add_example(select)
add_example(unbuffered)
