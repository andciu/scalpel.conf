# Scalpel Configuration File (`scalpel.conf`)

This file contains the customized configuration for the data recovery tool **Scalpel**, designed for forensic and targeted file carving operations.

## Purpose and Structure

The configuration is optimized for **selectivity** and **reliability**. By default, **all file types are disabled** (commented out with `#`) to ensure the scan is fast and focuses only on the formats of interest.

The file is divided into logical sections (Images, RAW, Documents, Databases, Archives, etc.) to facilitate easy activation.

## How to Use This Configuration

To perform a data recovery run:

Open the `scalpel.conf` file.
**Remove the comment character (`#`)** from the lines corresponding to the file formats you intend to recover (e.g., only `jpg` and `pdf`).
Execute Scalpel, specifying this configuration file (`-c`) and the desired output folder name (`-o`).

**Example:**

```bash
scalpel -c scalpel.conf disk.image.dd -o /path/to/put/the/recover
