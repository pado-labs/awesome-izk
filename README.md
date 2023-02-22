# Awesome-iZK
created for cryptography/web3/privacy builders (updating...)

Interactive zero-knowledge (iZK) proofs are another type of zero knowledge proof system, compared with the more well-known non-interactive versions (a.k.a, zk-SN(T)ARKs. Howeverm, iZK protocols shares the extra advantages including:

1. scalable for large statement
2. cheap computation and memory cost
3. avoid of trusted setup

with the requirement of "more interactions" -- the prover and the verifier execute in multiple rounds of communications. The interaction is quite like in MPC (secure multi-party computation), and in fact the cutting-edge iZK algorithms are built from MPC!

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


Check this [post](https://blog.chain.link/interactive-zero-knowledge-proofs/) for a more comprehensive understanding of iZK and NIZK.

## iZK related papers 
### General IZK protocols
* Wolverine (IEEE S&P' 21): https://eprint.iacr.org/2020/925  
* Quicksilver (CCS' 21): https://eprint.iacr.org/2021/076  
* Mystique (USENIX' 21): https://www.usenix.org/system/files/sec21-weng.pdf
* Mac'n'Cheese (CRYPT' 21): https://eprint.iacr.org/2020/1410
* Limbo (CCS' 21): https://eprint.iacr.org/2021/215
* zkCNN (CCS' 21): https://eprint.iacr.org/2021/673
* Appenzeller to Brie (CCS' 21): https://eprint.iacr.org/2021/750

### Related protocols
Vector Oblivious linear-function evaluation （VOLE）:
* CCS'18: https://eprint.iacr.org/2019/273

Information-theoretic message authentication codes(IT-MACs):
* Eurocrypt'11: https://eprint.iacr.org/2010/514.pdf
* CRYPT'12: https://eprint.iacr.org/2011/091
