project(RedHat.AspNetCore.Server.Kestrel.Transport.Linux.Native)

set(SOURCES
    pipeend.cpp
    epoll.cpp
    socket.cpp
    scheduler.cpp
    io.cpp
    error.cpp
    aio.cpp
)

add_library(RedHat.AspNetCore.Server.Kestrel.Transport.Linux.Native
    SHARED
    ${SOURCES}
)

install_library_and_symbols (RedHat.AspNetCore.Server.Kestrel.Transport.Linux.Native)