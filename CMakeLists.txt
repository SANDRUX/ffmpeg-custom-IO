cmake_minimum_required(VERSION 3.5)

project(ffmpeg-remuxer LANGUAGES C)

add_executable(ffmpeg-remuxer main.c)
target_link_libraries(${PROJECT_NAME} -lavformat -lavcodec -lavutil -lswresample -lz -lpthread -lm)

