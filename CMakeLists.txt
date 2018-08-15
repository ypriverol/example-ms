cmake_minimum_required(VERSION 3.12)
project(msCRUSH)

set(CMAKE_C_COMPILER  "${CMAKE_CXX_FLAGS} -Wall -std=c++11")

include_directories(src/app)
include_directories(src/class)
include_directories(src/test)
include_directories(src/utility)


add_executable(msCRUSH
        #src/app/generate_consensus_spectrum_for_mscrush.cc
        src/app/greedyCluster_omp_general_charge.cc
        src/class/core.cc
        src/class/core.h
        src/class/distance.cc
        src/class/distance.h
        src/class/params.h
        src/class/peak.h
        src/class/spectrum.h
        src/utility/io.cc
        src/utility/io.h
        src/utility/params.h
#        src/test/case_test.cc
##        src/test/consensus_test.cc
#        src/test/core_test.cc
#        src/test/cosine_test.cc
#        src/test/cosine_test_unit_test.cc
#        src/test/disk_io_speed_test.cc
#        src/test/distance_test.cc
#        src/test/greedyCluster.cc
#        src/test/io_multithread_test.cc
#        src/test/io_test.cc
#        src/test/memory_test.cc
#        src/test/merge_two_peaks_test.cc
#        src/test/peak_test.cc
#        src/test/pointer_test.cc
#        src/test/read_ms2_random_access.cc
#        src/test/read_speed_test.cc
#        src/test/spectrum_test.cc
#        src/test/split_large_mgf.cc
#        src/test/sscanf_test.cc
#        src/test/thread_test.cc
        )
