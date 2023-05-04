project(heatmap LANGUAGES C)

file(GLOB_RECURSE HEATMAP_COLORSCHEMES colorschemes/*.c)

add_library(heatmap heatmap.c ${HEATMAP_COLORSCHEMES})

target_include_directories(heatmap PUBLIC .)