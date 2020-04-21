add_library(hello hello.cpp) #(name, filename for *definition*)
add_library(blah blah.cpp)

add_executable(bin_main main.cpp) #(name, filename)
target_link_libraries(bin_main 
		      hello
		      blah) #first is receiver of link, second is library to link
