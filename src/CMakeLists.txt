
include_directories(
    ../include/nopoll
    ${TOPDIR}/prebuilts/openssl-1.1.0e/include
)

file(GLOB_RECURSE HEADERFILES "../include/*" "*.h")
AUX_SOURCE_DIRECTORY(. DIR_SRCS)
ADD_LIBRARY(nopoll ${DIR_SRCS} ${HEADERFILES})

