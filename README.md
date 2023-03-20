# Awesome-IZK
Created for Web3 builders. (Keep updating...)

Interactive Zero-Knowledge (IZK) proofs are another type of zero-knowledge proof system,in which the proof is consists of a multi-round protocol between the prover and verifier. It is also called as a designed verifier zero-knowledge protocol. It is a complement of zk-SNARKs/zk-STARKs.

IZK enjoys the following benefits, and we believe it will become a key building block for Web3 applications.

1. Scalable for large statements.
2. Cheap computation and memory cost.
3. No trusted setup.

With the requirement of "more interactions" -- the prover and the verifier execute in multiple rounds of communications. The interactions are quite like the ones in MPC (Secure Multi-Party Computation), for which in fact the cutting-edge IZK algorithms are built from MPC.

```
              xxx
            xxxxxxx                                         +---xxx
             |   | +----------+                             |   |  xx
             |   | | statement|  --------------------->     |   |   xxx
             +-+-+ +-+--------+                             +-+-+
               |     |          <----------------------       |
+---------+----+-----+                                  ------+---+------+
| secret  |    |                 --------------------->       |   |  Y/N |
+---------+    |                                           +--+   +------+
             +-+-+              <---------------------        |  |
             |   |                                         |  +---++
             |   |              ---------------------->    |      ++
             |   |
```

## Post
Here is a series of posts about IZK proofs presented by Chainlink.
* [Introduction to Interactive Zero-Knowledge Proofs](https://blog.chain.link/interactive-zero-knowledge-proofs/).
* [Background on Computation Complexity Metrics](https://blog.chain.link/computation-complexity-metrics/).
* [Commit-and-Prove ZKs](https://blog.chain.link/commit-and-prove-zks/).
* [VOLE-Based ZK](https://blog.chain.link/vole-based-zk/).
* [VOLE-Based Interactive Commitments](https://blog.chain.link/vole-based-interactive-commitments/).
* [Realizing VOLE](https://blog.chain.link/realizing-vole/).
* [Realizing SPVOLE](https://blog.chain.link/realizing-spvole/)

## Paper 
### Private Coin IZKs
* DILO22 (CCS'22): https://eprint.iacr.org/2022/552
* BBMS22 (CRYPTO'22): https://eprint.iacr.org/2022/819
* Wolverine (IEEE S&P' 21): https://eprint.iacr.org/2020/925  
* Quicksilver (CCS' 21): https://eprint.iacr.org/2021/076  
* Mystique (USENIX' 21): https://www.usenix.org/system/files/sec21-weng.pdf
* Mac'n'Cheese (CRYPTO' 21): https://eprint.iacr.org/2020/1410
* Limbo (CCS' 21): https://eprint.iacr.org/2021/215
* Appenzeller to Brie (CCS' 21): https://eprint.iacr.org/2021/750
* DIO21 (ITC'21): https://eprint.iacr.org/2020/1446
* FKL+21 (CCS'21):https://eprint.iacr.org/2021/979
* HYDK21 (IEEE S&P'21): https://eprint.iacr.org/2022/810
* HK20b (CCS'20): https://eprint.iacr.org/2022/809
* HK20a (EUROCRYPT'20): https://eprint.iacr.org/2020/136
* FNO15 (EUROCRYPT'15): https://eprint.iacr.org/2014/598
* JKO13 (CCS'13): https://eprint.iacr.org/2013/073

### Related protocols
Vector Oblivious Linear-function Evaluation （VOLE）:
* BCGI18(CCS'18): https://eprint.iacr.org/2019/273

Information-Theoretic Message Authentication Codes(IT-MACs):
* NNOB12 (CRYPTO'12): https://eprint.iacr.org/2011/091
* BDOZ11（EUROCRYPT'11）: https://eprint.iacr.org/2010/514.pdf
