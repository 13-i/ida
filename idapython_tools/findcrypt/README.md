# FindCrypt
A Python implementation of IDA FindCrypt/FindCrypt2 plugin (see http://www.hexblog.com/?p=28).

## How to use
Execute findcrypt.py on your IDA. Tested on IDA 7.0+ for macOS.

## Supported constants
* zlib: zinflate_lengthStarts, zinflate_lengthExtraBits, zinflate_distanceStarts, zinflate_distanceExtraBits, zdeflate_lengthCodes
* DES: DES_ip, DES_fp, DES_ei, DES_sbox[1-8], DES_p32i, DES_pc[1-2]
* AES: Rijndael_sbox, Rijndael_inv_sbox, Rijndael_Te[0-4], Rijndael_Td[0-4]
* Blowfish: Blowfish_P_array, Blowfish_S_boxes
* CRC32: CRC32_m_tab_le, CRC32_m_tab_be
* MD5: MD5_T, MD5_initstate
* SHA1: SHA1_H
* SHA224: SHA224_H
* SHA256: SHA256_K, SHA256_H
* SHA512: SHA512_K
* RC5_RC6: RC5_RC6_PQ
* Salsa20_ChaCha: Salsa20_ChaCha_sigma, Salsa20_ChaCha_tau
* Camellia: Camellia_sigma, Camellia_SBOX[1-4]
* Adler-32: Adler32_BASE
* (XX)TEA: (XX)TEA_delta
* xxHash32: xxHash32_PRIME32_[1-5]
* xxHash64: xxHash64_PRIME64_[1-5]

## Todo
1. Add more constants - I always welcome your pull request :)
2. Performance improvement
