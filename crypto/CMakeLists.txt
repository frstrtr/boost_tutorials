project(crypto)

set(HEADER_FILES
        common.h
        aes.h
        chacha20.h
        chacha_poly_aead.h
        hkdf_sha256_32.h
        hmac_sha256.h
        hmac_sha512.h
        poly1305.h
        ripemd160.h
        sha1.h
        sha256.h
        sha512.h
        siphash.h
        random.h
        uint256.h)
set(SOURCE_FILES
        aes.cpp
        chacha20.cpp
        chacha_poly_aead.cpp
        hkdf_sha256_32.cpp
        hmac_sha256.cpp
        hmac_sha512.cpp
        poly1305.cpp
        ripemd160.cpp
        sha1.cpp
        sha256.cpp
        sha256_avx2.cpp
        sha256_shani.cpp sha256_sse4.cpp
        sha256_sse41.cpp
        sha512.cpp
        siphash.cpp
        random.cpp
        uint256.cpp)

add_library(crypto STATIC ${SOURCE_FILES} ${HEADER_FILES})
