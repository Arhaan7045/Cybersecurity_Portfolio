EP-014

*Date:* 25 November 2026
*Topic:* Compression, Archives & Safe File Handling

*Topics learned:*
- Understanding the difference between archiving and compression.
- Common archive and compression formats.
- Creating TAR archives.
- Creating and extracting Gzip-compressed archives.
- Compressing and decompressing individual files.
- Listing and inspecting archive contents.
- Identifying file types using `file`.
- Checking storage usage and file sizes.
- Verifying file integrity using SHA-256 hashes.
- Extracting unknown archives safely.
- Understanding archive path traversal and compression bombs.
- **Linux commands learned:** `tar -cf`, `tar -czf`, `tar -tzf`, `tar -xzf`, `gzip`, `gunzip`, `file`, `sha256sum`, `du -sh`, `mktemp -d`.

*Cybersecurity lesson:* Handling investigation evidence safely, inspecting unknown archives before extraction, preventing unsafe file extraction and verifying file integrity using cryptographic hashes.

*Key takeaway:* Always inspect an archive before extracting it, use a dedicated extraction directory and verify important evidence using trusted hashes.
