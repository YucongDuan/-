# Contributing

Changes to protocol parsers, mappings, identity, MPI, consent, signatures, clinical staging or audit behavior must include:

1. a versioned interface or behavior contract;
2. synthetic test fixtures with no patient information;
3. normal, boundary, duplicate, malformed and rollback tests;
4. a statement of semantic residuals and clinical impact;
5. security and privacy review notes;
6. backward compatibility and migration notes.

No contribution may introduce default autonomous diagnosis, prescription or order submission. Site-specific credentials and endpoint parameters must never be committed.
