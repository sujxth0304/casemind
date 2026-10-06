# CASEMIND System Overview

## Purpose

CASEMIND is an AI-assisted investigative intelligence platform
designed to help analysts organize, correlate, search, and
reason over heterogeneous evidence.

## High-Level Architecture

```text
                 CASEMIND
                    |
          +---------+---------+
          |                   |
       Web App              API
      React/TS            FastAPI
                              |
              +---------------+---------------+
              |               |               |
          PostgreSQL        Neo4j           Redis
          + pgvector        Graph          Queue
              |
          Object Storage
              |
        Evidence Processing
              |
          AI/ML Services