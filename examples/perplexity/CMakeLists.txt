set(TARGET perplexity)
add_executable(${TARGET} perplexity.cpp)
target_link_libraries(${TARGET} PRIVATE common llama ggml ${CMAKE_THREAD_LIBS_INIT})
target_compile_features(${TARGET} PRIVATE cxx_std_11)
