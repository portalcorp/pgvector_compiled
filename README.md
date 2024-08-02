# pgvector_compiled

Precompiled OS packages (zips) for pgvector on Linux, MacOS, and Windows.

The [Releases](https://github.com/portalcorp/pgvector_compiled/releases) page contains the compiled versions of pgvector for PostgreSQL 16.
The version number format is `v0.<POSTGRESQL_VERSION>.<INCREMENT>` where increments increases by one for commit to this repo.

## Usage

1. Download the zip for your OS from the [Releases](https://github.com/portalcorp/pgvector_compiled/releases) page.

2. Extract the zip to get the `sql` folder.

3. Add the files to your PostgreSQL installation folders:

Here are the markdown bullet point lists of the files for each OS, showing the relative paths within the created zip file:

### Linux

- `/include/server/extension/vector/*.h`
- `/lib/bitcode/vector.index.bc`
- `/lib/bitcode/vector/src/*.bc`
- `/lib/vector.so`
- `/share/extension/vector*.sql`
- `/share/extension/vector.control`

### macOS

- `/lib/vector.dylib`
- `/lib/vector.so` (not needed)
- `/share/extension/vector*.sql`
- `/share/extension/vector.control`
- `/include/server/extension/vector/*.h`

### Windows

- `/lib/vector.dll`
- `/share/extension/vector*.sql`
- `/share/extension/vector.control`
- `/include/server/extension/vector/halfvec.h`
- `/include/server/extension/vector/sparsevec.h`
- `/include/server/extension/vector/vector.h`
