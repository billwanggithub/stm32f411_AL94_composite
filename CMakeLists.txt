cmake_minimum_required(VERSION 3.15)

project(stm32f411_composite LANGUAGES C CXX ASM)

find_bsp(ID com.sysprogs.project_importers.stm32.cubemx SOURCE_PROJECT stm32f411_composite.ioc)

add_bsp_based_executable(NAME stm32f411_composite
	GENERATE_BIN
	GENERATE_MAP)

