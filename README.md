# pgvector_compiled

Precompiled OS packages (zips) for pgvector on Linux, MacOS, and Windows.

## Usage

1. Download the zip for your OS from the [Releases](https://github.com/portalcorp/pgvector_compiled/releases) page.

2. Extract the zip to get the `sql` folder.

3. Add the files to your PostgreSQL installation folders:

### Linux

```bash
cp sql/vector--0.5.1.sql $PG_DIR/share/extension/vector--0.5.1.sql
cp vector.control $PG_DIR/share/extension/vector.control
cp vector.so $PG_DIR/lib/vector.so
```

### MacOS

```bash
cp sql/vector--0.5.1.sql $PG_DIR/share/extension/vector--0.5.1.sql
cp vector.control $PG_DIR/share/extension/vector.control
cp vector.so $PG_DIR/lib/vector.so
```

### Windows

```bash
cp sql/vector--0.5.1.sql $PG_DIR/share/extension/vector--0.5.1.sql
cp vector.control $PG_DIR/share/extension/vector.control
cp vector.dll $PG_DIR/bin/vector.dll
```
