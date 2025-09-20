cmake_minimum_required(VERSION 3.10)
project(cbm6502asm)
set(SRC_FILES 
src/asm.c
src/asm.h
src/direct1.c
src/direct2.c
src/express.c
src/help.c
src/line.c
src/macrodef.c
src/opcode.c
src/outline.c
src/pass1.c
src/pass2.c
src/symbol.c
src/template.h
)


add_executable(${PROJECT_NAME} ${SRC_FILES})
target_compile_definitions(${PROJECT_NAME} PRIVATE _CRT_SECURE_NO_WARNINGS)

