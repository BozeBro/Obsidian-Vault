#Hashing 
[[Simple Uniform Hashing Assumption]]

We use the hash function and then increment by 1 until we find an available location.  We assume $n > 2m$

We'll use a tombstone to mark empty cells created by deletion. So we don't stop at empty cell if key already exists somewhere else. 