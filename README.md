# Storage Papers

A living collection of data storage research papers, organized by topic: distributed filesystems, key-value stores and LSM-trees, consensus and replication, erasure coding, flash/NVMe, caching and tiering, cloud and disaggregated storage, storage engines, persistent memory, and vector search indexes. Updated daily from the morning sweep — new papers land in the topic file that matches their primary angle, with the PDF in [`papers/`](papers/).

## Topics

- [Distributed Filesystems & Object Storage](topics/distributed-filesystems.md) — Distributed filesystems and object stores: GFS, HDFS, Ceph, photo and warm BLOB storage, and metadata scaling. (22 papers)
- [Key-Value Stores & LSM Trees](topics/key-value-lsm.md) — Key-value stores and LSM-trees: Dynamo, Bigtable, Cassandra, LevelDB/RocksDB lineage, learned indexes, and compaction design. (25 papers)
- [Consensus, Replication & Distributed Transactions](topics/consensus-replication.md) — Consensus and replication: Lamport clocks, Paxos, Raft, BFT, Spanner, and geo-distributed transactions. (23 papers)
- [Erasure Coding, Durability & Repair](topics/erasure-coding.md) — Erasure coding and durability: Reed-Solomon, RAID, regenerating codes, LRC, and field studies of disk and data corruption. (19 papers)
- [Flash / SSD / NVMe](topics/flash-ssd-nvme.md) — Flash storage: FTLs, write amplification, ZNS, open-channel SSDs, SPDK, NVMe-oF, and SSD field studies. (21 papers)
- [Caching, Tiering & Memory Hierarchy](topics/caching-tiering.md) — Caching and tiering: replacement policies, memcached at scale, hybrid DRAM/SSD caches, and burst buffers. (18 papers)
- [Cloud, Block & Disaggregated Storage](topics/cloud-block-disaggregated.md) — Cloud and disaggregated storage: Azure Storage, RDMA far memory, CXL memory pooling, and serverless storage. (17 papers)
- [Storage Engines, Indexing & Persistent Memory](topics/storage-engines-persistent-memory.md) — Storage engines and persistent memory: B-trees, latch-free indexes, PM filesystems, and near-data processing. (17 papers)
- [Vector Search Indexes](topics/vector-search-indexes.md) — Graph and partition-based approximate nearest neighbor indexes and vector quantization: HNSW, DiskANN, Faiss, ScaNN, and the quantizers behind them. (14 papers)
- [Recent Work 2023–2026](topics/recent-work.md) — Recent storage work (2023–2026) from arXiv and OSDI/SOSP/FAST/NSDI/ATC proceedings, newest first within each tier. (45 papers)

## Adding papers

Each paper goes in `papers/` (kebab-case filename with arXiv ID) and gets a row in its primary topic's table with an arXiv link, authors, date added, an Importance score (see below), and a one-line summary. Entries are not constrained to arXiv: a work published only as a conference paper, technical report, or other primary source gets a row linking that source, with no PDF required. Insert the row in the table's reading order: by Importance first, then foundational-before-recent within the same tier (newest first within a tier for Recent Work).

## Importance

Every paper carries an Importance score for a reader working through data storage engineering, and each topic table is sorted in reading order — most important first, with foundational/canonical works ahead of later papers within the same tier.

- ★★★★★ — field-defining: introduced the technique, or the canonical reference later work builds on
- ★★★★☆ — major: widely cited or adopted, benchmark-setting, or used in production systems
- ★★★☆☆ — solid: a real method or result worth reading
- ★★☆☆☆ — incremental: a small improvement, or narrow in scope/applicability
- ★☆☆☆☆ — tangential: marginal relevance to storage engineering

## Stats

- 235 papers across 10 topics as of 2026-11-09
- 62 PDFs in papers/ (arXiv papers only; venue papers link to their open-access source)
