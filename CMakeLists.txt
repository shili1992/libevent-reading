cmake_minimum_required(VERSION 3.10)
project(libevent_comment C)

set(CMAKE_C_STANDARD 11)

include_directories(.)
include_directories(compat)
include_directories(compat/sys)
include_directories(sample)
include_directories(test)

add_executable(libevent_comment
        compat/sys/_libevent_time.h
        compat/sys/queue.h
        sample/event-test.c
        sample/signal-test.c
        sample/time-test.c
        test/bench.c
        test/regress.c
        test/regress.gen.c
        test/regress.gen.h
        test/regress.h
        test/regress_dns.c
        test/regress_http.c
        test/regress_rpc.c
        test/test-eof.c
        test/test-init.c
        test/test-time.c
        test/test-weof.c
        buffer.c
        config.h
        devpoll.c
        epoll.c
        epoll_sub.c
        evbuffer.c
        evdns.c
        evdns.h
        event-internal.h
        event.c
        event.h
        event_tagging.c
        evhttp.h
        evport.c
        evrpc-internal.h
        evrpc.c
        evrpc.h
        evsignal.h
        evutil.c
        evutil.h
        http-internal.h
        http.c
        kqueue.c
        log.c
        log.h
        min_heap.h
        poll.c
        select.c
        signal.c
        strlcpy-internal.h
        strlcpy.c)
