cmake_minimum_required(VERSION 3.10)
project(VulkanPractice VERSION 0.0.1)

find_package(Vulkan REQUIRED)

add_executable(VulkanPractice VulkanPractice.cc)

target_link_libraries(VulkanPractice PRIVATE Vulkan::Vulkan)