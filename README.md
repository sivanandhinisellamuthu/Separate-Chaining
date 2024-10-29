# Bucket Hashing: A Collision-Resolution Algorithm for Hash Tables

## Overview
**Bucket Hashing** (also known as **Separate Chaining**) is a robust technique for handling collisions in hash tables. Instead of overwriting or probing for new slots when multiple keys map to the same index, Bucket Hashing stores these keys in a "bucket," typically implemented as a linked list or dynamic array. This allows multiple keys to reside at the same index, ensuring constant-time complexity for insertions and lookups in ideal conditions.

## Key Features
- **Collision Handling**: Efficiently resolves hash collisions using separate chains (buckets) without degrading hash table performance.
- **Flexible Storage**: Buckets at each hash table index can be implemented using different data structures, such as linked lists or dynamic arrays.
- **Scalable Performance**: Bucket Hashing maintains stable performance even when the load factor increases, as bucket size can dynamically expand.
## Why Bucket Hashing?
When using a hash table, collisions are inevitable due to limited space. Bucket Hashing offers a scalable and flexible solution to store multiple elements at the same index. Unlike open addressing techniques, it prevents primary clustering and minimizes search times during collisions.

## Usage
To implement **Bucket Hashing**, we:
1. Use a primary hashing algorithm (like division or multiplication) to map keys to table indices.
2. At each index, maintain a bucket (e.g., a linked list) that stores keys that hash to the same value.
3. Insertion, deletion, and search operations are performed within the bucket if collisions occur.

