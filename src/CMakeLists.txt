set(RADV_PUBLIC_HEADERS radv.h)
set(RADV_SOURCE radv.c)

add_executable(radv ${RADV_PUBLIC_HEADERS} ${RADV_SOURCE})

set_target_properties(
    radv
    PROPERTIES
    PUBLIC_HEADER ${RADV_PUBLIC_HEADERS}
    C_STANDARD 99
)

install(TARGETS radv)
