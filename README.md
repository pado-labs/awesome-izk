# Awesome-iZK
created for cryptography/web3/privacy builders (updating...)

Interactive zero-knowledge (iZK) proofs are another type of zero-knowledge proof system, compared with the more well-known non-interactive versions, a.k.a, zk-SN(T)ARKs. However, iZK protocols share the extra advantages including:

1. scalable for large statements
2. cheap computation and memory cost
3. avoid of trusted setup

With the requirement of "more interactions" -- the prover and the verifier execute in multiple rounds of communications. The interactions are quite like the ones in MPC (Secure Multi-Party Computation), for which in fact the cutting-edge iZK algorithms are built from MPC.

```
              xxx
            xxxxxxx                                         +---xxx
             |   | +----------+                             |   |  xx
             |   | | statement|  --------------------->     |   |   xxx
             +-+-+ +-+--------+                             +-+-+
               |     |         <-----------------------       |
+---------+----+-----+                                  ------+---+------+
| secret  |    |           --------------------------->       |   |  Y/N |
+---------+    |                                           +--+   +------+
             +-+-+     <--------------------------------   |  |
             |   |                                         |  +---++
             |   |    --------------------------------->   |      ++
             |   |
```


Check this [post](https://blog.chain.link/interactive-zero-knowledge-proofs/) for more comprehensive understandings of iZK and NIZK.

## Related papers 
### General iZK protocols
* Wolverine (IEEE S&P' 21): https://eprint.iacr.org/2020/925  
* Quicksilver (CCS' 21): https://eprint.iacr.org/2021/076  
* Mystique (USENIX' 21): https://www.usenix.org/system/files/sec21-weng.pdf
* Mac'n'Cheese (CRYPTO' 21): https://eprint.iacr.org/2020/1410
* Limbo (CCS' 21): https://eprint.iacr.org/2021/215
* Appenzeller to Brie (CCS' 21): https://eprint.iacr.org/2021/750

### Line-Point ZK protocols
* DIO21 (ITC'21): https://eprint.iacr.org/2020/1446
* FKL+21 (CCS'21):https://eprint.iacr.org/2021/979
* DILO22 (CCS'22): https://eprint.iacr.org/2022/552
* BBMS22 (CRYPTO'22): https://eprint.iacr.org/2022/819

### Some Classic iZK protocols
* JKO13 (CCS'13): https://eprint.iacr.org/2013/073
* FNO15 (EUROCRYPT'15): https://eprint.iacr.org/2014/598
* HK20a (EUROCRYPT'20): https://eprint.iacr.org/2020/136
* HYDK21 (IEEE S&P'21): https://eprint.iacr.org/2022/810
* HK20b (CCS'20): https://eprint.iacr.org/2022/809

### Related protocols
Vector Oblivious linear-function evaluation （VOLE）:
* BCGI18(CCS'18): https://eprint.iacr.org/2019/273

Information-theoretic message authentication codes(IT-MACs):
* BDOZ11（EUROCRYPT'11）: https://eprint.iacr.org/2010/514.pdf
* NNOB12 (CRYPTO'12): https://eprint.iacr.org/2011/091
