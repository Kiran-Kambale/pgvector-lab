AI Skills Roadmap for a PostgreSQL DBA
pgvector, Vector Databases and RAG --- A 10-Week Free Learning Plan
Prepared for: Kiran
Start date: 8 October 2026
Daily commitment: 1.5--2 hours

A practical roadmap for a PostgreSQL DBA to build skills in AI
fundamentals, embeddings, vector search, pgvector, Retrieval-Augmented
Generation (RAG), and production operations for vector workloads.
Why This Skill?
Vector search with pgvector is a natural AI skill for a PostgreSQL
DBA. It builds on existing database knowledge, and teams running AI
features on PostgreSQL need people who can index, tune, back up, and
monitor vector workloads in production.
Roadmap Overview
  Weeks                   Focus                   What you'll learn
  1--2                    AI/ML basics            Embeddings, LLMs, RAG,
                                                  and vector database
                                                  concepts

  3--4                    Python essentials       psycopg, pandas, API
                                                  calls, and
                                                  sentence-transformers

  5--6                    pgvector hands-on     Store embeddings,
                                                  similarity search, and
                                                  IVFFlat vs. HNSW tuning

  7--8                    RAG project             Chunking, embeddings,
                                                  storage, hybrid search,
                                                  and answers with a local
                                                  LLM

  9--10                   DBA production topics   Index memory, vacuum,
                                                  backup, replication,
                                              monitoring, and scaling
Free Learning Resources
- Generative AI for Everyone --- DeepLearning.AI on Coursera (audit
  for free)
- Intro to Large Language Models --- Andrej Karpathy (YouTube)
- Vector Databases: From Embeddings to Applications ---
  DeepLearning.AI short course
- Building Applications with Vector Databases --- DeepLearning.AI
  short course
- Python for Everybody --- freeCodeCamp / Coursera audit
- Hugging Face free NLP / LLM course
- Microsoft Generative AI for Beginners (GitHub)
- pgvector GitHub README, plus free Supabase and Neon pgvector
  guides
- Ollama for running free local LLMs on your own machine
How to Use This Plan
- [ ] Plan for 1.5--2 hours every day. If you miss a day, continue
  where you stopped rather than skipping tasks.
- [ ] Tick off each day's task as you complete it.
- [ ] Every seventh day is a review and writing day.
- [ ] Keep scripts in one GitHub repository (for example,
  pgvector-lab) and commit daily.
- [ ] Write what you learn as blog posts on your Sphinx site. These
  posts provide evidence of your skills to employers.
- [ ] Maintain notes on each error you encounter and how you fixed it.
  Production-style troubleshooting is an important skill.
Portfolio Deliverables
By Day 56, aim to have:
- [ ] A GitHub repository with scripts and a clear README
- [ ] Three blog posts:
  - [ ] Comparing pgvector indexes
  - [ ] Recall vs. latency tuning
  - [ ] Running RAG on PostgreSQL
- [ ] A short architecture diagram of your RAG setup
- [ ] An updated resume and LinkedIn profile mentioning pgvector,
  RAG, and vector search tuning
Day-by-Day Learning Plan
Week 1 --- AI Basics (Days 1--7)
Goal: Understand what LLMs, embeddings, and RAG are.
- [ ] Day 1 --- Setup day: Install Docker, Python 3.11+, and Git.
  Create a virtual environment and a GitHub repository called
  pgvector-lab. Start Week 1 of Generative AI for Everyone.
- [ ] Day 2: Finish Week 1 of Generative AI for Everyone. Write
  five lines explaining what an LLM is, what tokens are, and what a
  prompt is.
- [ ] Day 3: Start DeepLearning.AI's Vector Databases: From
  Embeddings to Applications. Complete Lessons 1--2 on embeddings.
- [ ] Day 4: Watch Andrej Karpathy's Intro to Large Language
  Models (about one hour). Take notes on how LLMs are trained and
  used.
- [ ] Day 5: Study Week 2 of Generative AI for Everyone. Explain
  RAG in your own words: retrieve, augment, generate.
- [ ] Day 6: Install Ollama and run a small local model, such as
  llama3.2 or mistral. Ask it 10 PostgreSQL questions and note
  incorrect answers.
- [ ] Day 7 --- Review: Write a one-page summary of AI concepts
  for a DBA. Use it as the draft for your first blog post.
Week 2 --- Vector Database Concepts (Days 8--14)
Goal: Learn how similarity search works before using pgvector.
- [ ] Day 8: Continue the Vector Databases course, Lessons 3--4,
  covering similarity metrics.
- [ ] Day 9: Compare cosine, L2, and inner product with a small
  NumPy example using three vectors.
- [ ] Day 10: Finish the Vector Databases course. Note the
  difference between exact search and approximate nearest-neighbor
  (ANN) search.
- [ ] Day 11: Start the Hugging Face LLM course, Chapters 1--2, to
  learn what transformers do.
- [ ] Day 12: Study Microsoft Generative AI for Beginners lessons
  on prompt engineering and RAG.
- [ ] Day 13: Read the pgvector README fully. List its data
  types, operators, and index types.
- [ ] Day 14 --- Review: Draw the RAG flow: documents → chunks →
  embeddings → database → LLM. Quiz yourself without notes.
Week 3 --- Python Essentials (Days 15--21)
Goal: Write small scripts that communicate with PostgreSQL and APIs.
- [ ] Day 15: Study variables, strings, and conditions in Python
  for Everybody. Complete five small exercises.
- [ ] Day 16: Practise loops, lists, and dictionaries. Write a
  script that counts words in a text file.
- [ ] Day 17: Learn functions and file reading/writing. Refactor
  the previous day's script into functions.
- [ ] Day 18: Work with JSON and the requests library. Call a
  free public API and print the result.
- [ ] Day 19: Install psycopg. Connect to PostgreSQL in Docker,
  create a table, and run INSERT and SELECT from Python.
- [ ] Day 20: Learn pandas basics: read a CSV, clean it, and load
  it into PostgreSQL.
- [ ] Day 21 --- Review: Build a mini-script that loads a CSV into
  PostgreSQL and runs three analysis queries. Commit it to GitHub.
Week 4 --- Embeddings in Python (Days 22--28)
Goal: Generate embeddings and prepare a dataset.
- [ ] Day 22: Install sentence-transformers. Embed 20 sentences
  with all-MiniLM-L6-v2 and print the vector size (384).
- [ ] Day 23: Compute cosine similarity between sentences in
  Python and identify the nearest matches.
- [ ] Day 24: Call Ollama from Python using its HTTP API. Send a
  prompt and print the answer.
- [ ] Day 25: Choose a dataset, such as your Sphinx blog pages or
  a public text dataset. Download and clean it.
- [ ] Day 26: Split text into chunks of 300--500 tokens with
  overlap. Write a reusable chunking function.
- [ ] Day 27: Embed 1,000 chunks, save them to a file, and measure
  processing time.
- [ ] Day 28 --- Checkpoint: Explain embeddings, vector search,
  and RAG aloud in five minutes. Identify and improve weak areas.
Week 5 --- pgvector Basics (Days 29--35)
Goal: Store embeddings in PostgreSQL and run similarity queries.
- [ ] Day 29 --- Lab 1: Run PostgreSQL 16 or 17 with pgvector in
  Docker. Execute CREATE EXTENSION vector and check the version.
- [ ] Day 30 --- Lab 2: Create a table with a vector(384) column
  plus text and metadata columns.
- [ ] Day 31 --- Lab 2 continued: Insert about 10,000 embedded
  rows from your dataset using psycopg batch inserts.
- [ ] Day 32 --- Lab 3: Run similarity queries using L2, cosine,
  and inner-product operators. Compare the top five results.
- [ ] Day 33: Run EXPLAIN ANALYZE on each query. Note that
  queries use a sequential scan when no index is present.
- [ ] Day 34: Add WHERE filters on metadata columns to
  vector-search queries. Test results and timing.
- [ ] Day 35 --- Review: Draft Blog Post 1: Getting Started with
  pgvector for DBAs.
Week 6 --- Indexing and Tuning (Days 36--42)
Goal: Compare IVFFlat and HNSW and measure recall.
- [ ] Day 36: Scale the table to 100,000--500,000 rows. Record
  baseline query latency without an index.
- [ ] Day 37 --- Lab 4: Build an IVFFlat index. Record build time
  and index size.
- [ ] Day 38: Tune IVFFlat by changing lists and probes.
  Record latency for each setting.
- [ ] Day 39 --- Lab 5: Build an HNSW index. Record build time,
  index size, and maintenance_work_mem used.
- [ ] Day 40: Tune HNSW by changing m, ef_construction, and
  hnsw.ef_search. Record latency.
- [ ] Day 41 --- Lab 6: Measure recall by comparing indexed
  results with exact results. Build a speed-versus-recall table.
- [ ] Day 42 --- Review: Publish Blog Post 2: pgvector Indexes
  Compared: IVFFlat vs. HNSW.
Week 7 --- Build the RAG Project (Days 43--49)
Goal: Build a working "Ask My Docs" system on PostgreSQL.
- [ ] Day 43 --- Lab 7: Create an ingestion script that reads PDFs
  or Markdown files from a documents folder.
- [ ] Day 44: Chunk, embed, and store documents with metadata such
  as source, page, and creation date.
- [ ] Day 45: Test retrieval quality by asking 10 questions and
  checking whether the correct chunks are returned.
- [ ] Day 46 --- Lab 8: Add full-text search using tsvector and
  a GIN index to the same table.
- [ ] Day 47: Combine full-text ranking and vector similarity into
  a hybrid-search query.
- [ ] Day 48 --- Lab 9: Pass the top five chunks to a local Ollama
  model as context and generate answers.
- [ ] Day 49 --- Review: Publish Blog Post 3: Running RAG on
  PostgreSQL. Push all code and the README to GitHub.
Week 8 --- Production-Style DBA Work (Days 50--56)
Goal: Test vector workloads under real DBA conditions.
- [ ] Day 50 --- Lab 10: Load-test vector queries using custom
  pgbench scripts or Locust.
- [ ] Day 51: Monitor pg_stat_statements, cache hit ratio, and
  memory during load testing. Record bottlenecks.
- [ ] Day 52 --- Lab 11: Run heavy updates and deletes on the
  vector table. Check bloat and vacuum behaviour.
- [ ] Day 53: Take pg_dump and pg_basebackup backups. Record
  backup size and restore time.
- [ ] Day 54 --- Lab 12: Set up a streaming replica and confirm
  that vector queries work on the standby.
- [ ] Day 55: Try table partitioning and read about
  pgvectorscale for larger datasets.
- [ ] Day 56 --- Review: Write a runbook for operating pgvector
  in production, covering sizing, tuning, backups, and monitoring.
Week 9 --- Production Depth (Days 57--63)
Goal: Learn to handle problems encountered in real vector databases.
- [ ] Day 57: Tune index builds using maintenance_work_mem and
  parallel maintenance workers. Compare build time and index size.
- [ ] Day 58: Reduce storage using halfvec or quantization
  options. Measure the impact on recall.
- [ ] Day 59: Review security: roles and row-level security for
  multi-tenant embeddings.
- [ ] Day 60: Monitor with postgres_exporter, Prometheus, and
  Grafana. Add panels for latency and index size.
- [ ] Day 61: Study high availability with Patroni and replica
  routing for vector workloads.
- [ ] Day 62: Plan upgrades and re-embedding: understand what
  happens when the embedding model changes.
- [ ] Day 63 --- Review: Update your runbook with these topics and
  test one failure scenario, such as replica failover.
Week 10 --- Next-Level Skills and Career (Days 64--70)
Goal: Turn learning into job-ready evidence.
- [ ] Day 64: Learn MLOps basics. Read about MLflow and how models
  are versioned and deployed.
- [ ] Day 65: Try an LLM-assisted query-tuning workflow: provide
  EXPLAIN output to an LLM and verify its advice.
- [ ] Day 66: Explore managed vector options such as Neon,
  Supabase, and cloud PostgreSQL. Compare them with self-hosted
  deployments.
- [ ] Day 67: Polish this GitHub README with an architecture
  diagram, benchmark tables, and instructions for running the project.
- [ ] Day 68: Update your resume and LinkedIn profile to include
  pgvector, RAG, vector-index tuning, and blog links.
- [ ] Day 69: Share your blog posts and repository on LinkedIn.
  Start applying to roles mentioning pgvector or AI data platforms.
- [ ] Day 70 --- Review: Plan the next 10 weeks. Choose one focus:
  MLOps, LLM observability, or advanced PostgreSQL internals.
Completion Checklist
- [ ] Complete the daily learning tasks
- [ ] Commit scripts and notes to GitHub
- [ ] Build and benchmark a pgvector dataset
- [ ] Compare IVFFlat and HNSW using measured results
- [ ] Build a working RAG application on PostgreSQL
- [ ] Document production operations in a runbook
- [ ] Publish three technical blog posts
- [ ] Update resume and LinkedIn with demonstrable project work
This README is a Markdown version of the learning plan. Tick the
checkboxes as you progress and add your own scripts, benchmark results,
notes, and architecture diagram to the repository.
