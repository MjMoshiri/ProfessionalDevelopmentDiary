### Data Handling Process

1. Session Manager receives data.
2. Data moves to the appropriate node via interconnect.
3. Data goes to the data module and then to NVRAM.
4. Client will be informed.
4. Efficiency Layer
5. Disk Writing

### Moving to Disk Process

1. Tetris Blocks are created.
2. Parities are calculated by the RAID manager.
3. Data is written into consistency points.
4. NVRAM can be flushed.

## File System Details

## Redundant Array of Independent/Inexpensive Disks (RAID)
- **Levels**:
    - 0: No Mirroring or Parity.
    - 1: Mirroring.
    - 4: Block-Level Striping with Dedicated Parity.
    - 5: Block-Level Striping with Distributed Parity.
    - 6: Block-Level Striping with Double Distributed Parity.
    - 10: 1 + 0.

### Inode Structure
- **Total Size**: 192 bytes.
  - **Metadata**: 128 bytes (owner, size, permissions, etc.)
  - **Data**: 64 bytes. (4KB block pointers, direct, indirect).

## Storage Techniques
- **Thin Provisioning**: Allocating storage space in a flexible manner.
- **Compaction**: Can be inline and/or post-process (adaptive 8KB blocks 50%, secondary 32KB blocks 25%). 

## Recovery Objectives
- **Recovery Point Objective (RPO)**:  maximum amount of data loss an organization can tolerate after an unplanned event.
- **Recovery Time Objective (RTO)**: maximum amount of time it takes to restore before it negatively impacts an organization's mission or business processes.
