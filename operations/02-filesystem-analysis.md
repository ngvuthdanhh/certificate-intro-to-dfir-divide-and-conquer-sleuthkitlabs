# 02 — Filesystem Analysis

## Partition & Volume Identification
- Identify partition table type.
- Locate active, hidden, or suspicious partitions.

## Filesystem Triage Logic
- NTFS: MFT, $LogFile, $UsnJrnl  
- FAT: directory entries & allocation tables  
- EXT: inodes, journals, block groups  
- APFS: snapshots, containers, volumes

## Metadata Interpretation
- Extract filename, inode, timestamps.
- Understand MACB timestamp semantics.
- Detect timestamp anomalies or manipulation.

## Deleted-File Reasoning Model
- Check allocation status.
- Examine metadata remnants.
- Cross-check with logs and timeline.

## File-Carving Decision Tree
- Identify magic headers/footers.
- Rebuild fragmented objects when possible.
- Assess carving reliability per file type.

## Anti-Forensics Indicators
- Timestamp clusters that defy system patterns.
- Excessive zeroed regions.
- Unexpected format or partition changes.
