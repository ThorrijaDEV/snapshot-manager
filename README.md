# Snapshot Manager — GUI for Snapper

A graphical snapshot management tool for Snapper on Omarchy and Arch Linux, providing an intuitive interface for creating, browsing, and managing system snapshots.

## What is it?

A Python/tkinter GUI application that wraps Snapper (the Btrfs snapshot manager used by Omarchy and openSUSE) to make snapshot operations accessible without memorizing CLI commands. Designed for Omarchy/Arch systems using Btrfs with Snapper configured.

## What does it do?

- **List and browse** existing snapshots with metadata (date, type, description, cleanup algorithm)
- **Create new snapshots** with custom descriptions (pre, post, single)
- **Delete unwanted snapshots** safely with confirmation
- **View snapshot details** and metadata
- **Rollback to previous snapshots** (with appropriate warnings)
- **Mount/unmount snapshots** for file access and recovery
- **Integration with omarchy-snapshot** for Omarchy systems
- **Progress indicators** and status updates during operations

## Technologies

Python 3.x, tkinter (stdlib), Snapper (system dependency), python-psutil (optional, for system monitoring)

## Installation

### Dependencies

- Python 3.x
- python-psutil (for system monitoring, optional but recommended)
- python-tkinter (for GUI interface)
- snapper (must be installed and configured on the system)

### Install from source

```bash
git clone https://github.com/ThorrijaDEV/snapshot-manager
cd snapshot-manager
make install
```

## Usage

Run the snapshot manager:

```bash
snapper-manager
```

Note: Running with sudo is required for most snapshot operations.

## Configuration

The snapshot manager can be configured by editing `config.json` in the installation directory.

## Status

**Functional / Maintenance**

Working GUI for Snapper operations on Omarchy/Arch. Core features implemented: list, create, delete, rollback, mount/unmount.

## Repository Note

This repository contains documentation only. The implementation is private code.

## License

MIT