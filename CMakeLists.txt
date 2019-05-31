cmake_minimum_required(VERSION 2.6)
project(bwa)

set(CMAKE_CXX_COMPILER /usr/bin/gcc)

add_custom_target(BWA cd ${PROJECT_SOURCE_DIR} && make VERBATIM)
add_custom_target(BWA-clean cd ${PROJECT_SOURCE_DIR} && make clean VERBATIM)



set(SOURCE_FILES
        "bamlite.c"
        "bwa.c"
        "bwamem_extra.c"
        "bwape.c"
        "bwaseqio.c"
        "bwtaln.c"
        "bwtgap.c"
        "bwtindex.c"
        "bwtsw2_aux.c"
        "bwtsw2_core.c"
        "bwtsw2_pair.c"
        "fastmap.c"
        "kopen.c"
        "ksw.c"
        "main.c"
        "maxk.c"
        "QSufSort.c"
        "rope.c"
        "bntseq.c"
        "bwamem.c"
        "bwamem_pair.c"
        "bwase.c"
        "bwashm.c"
        "bwt.c"
        "bwt_gen.c"
        "bwt_lite.c"
        "bwtsw2_chain.c"
        "bwtsw2_main.c"
        "example.c"
        "is.c"
        "kstring.c"
        "kthread.c"
        "malloc_wrap.c"
        "pemerge.c"
        "rle.c"
        "utils.c"
        )

add_executable(FakeTarget ${SOURCE_FILES})