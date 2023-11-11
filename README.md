# Minirel HeapFile Manager

## Description

The Minirel HeapFile Manager is a component of the Minirel database management system, designed to manage heap files and provide mechanisms for record insertion, deletion, and scanning with optional filtering. This project implements the logical layer over the physical pages provided by the Minirel database's I/O layer.

## Features

- **FileHdrPage Class**: Manages the header page of each heap file, containing metadata such as file name, page count, and record count.
- **HeapFile Class**: Provides methods for inserting and deleting records in a heap file.
- **HeapFileScan Class**: Extends HeapFile, offering scanning capabilities with optional search predicates.
- **InsertFileScan Class**: Derived from HeapFile for record insertion.


## Usage

Explain how to use your project, including basic usage examples.

```cpp
// Example of creating a heap file
createHeapFile("sample_heapfile");

// Example of using HeapFileScan
HeapFileScan scanner("sample_heapfile", status);
scanner.startScan(...);
// ...
scanner.endScan();

