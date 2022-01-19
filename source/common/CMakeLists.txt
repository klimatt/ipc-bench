###########################################################
## SOURCES
###########################################################

set(IPC_BENCH_COMMON_SOURCES
	utility.c
	benchmarks.c
	signals.c
	arguments.c
	process.c
	sockets.c
	parent.c
)

###########################################################
## TARGETS
###########################################################

add_library(ipc-bench-common STATIC ${IPC_BENCH_COMMON_SOURCES})
target_compile_options(ipc-bench-common PUBLIC -fPIC)
