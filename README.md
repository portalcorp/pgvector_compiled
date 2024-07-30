# pgvector_compiled

Precompiled OS packages (zips) for pgvector on Linux, MacOS, and Windows.

## Usage

1. Download the zip for your OS from the [Releases](https://github.com/portalcorp/pgvector_compiled/releases) page.

2. Extract the zip to get the `sql` folder.

3. Add the files to your PostgreSQL installation folders:

### Linux

```bash
cp -r pgvector-linux-pg16/sql $PG_DIR/share/extension/
cp pgvector-linux-pg16/vector.control $PG_DIR/share/extension/
cp pgvector-linux-pg16/vector.so $PG_DIR/lib/
```

### MacOS

```bash
cp -r pgvector-macos-pg16/sql $PG_DIR/share/extension/
cp pgvector-macos-pg16/vector.control $PG_DIR/share/extension/
cp pgvector-macos-pg16/vector.dylib $PG_DIR/lib/
```

### Windows

```bash
cp -r pgvector-windows-pg16/sql $PG_DIR/share/extension/
cp pgvector-windows-pg16/vector.control $PG_DIR/share/extension/
cp pgvector-windows-pg16/vector.dll $PG_DIR/bin/
```
