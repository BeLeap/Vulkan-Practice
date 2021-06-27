cmake_minimum_required(VERSION 3.10)
project(VulkanPractice VERSION 0.0.1)

find_package(Vulkan REQUIRED)
find_package(glfw3 CONFIG REQUIRED)

add_executable(main main.cc)

target_link_libraries(main PRIVATE Vulkan::Vulkan)
target_link_libraries(main PRIVATE glfw)