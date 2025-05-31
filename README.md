# NES CHR Editor Extended 🎮 - Overview

This document outlines the features and user interface of the "NES CHR Editor Extended," based on the provided text. It appears to be a tool designed for creating and editing CHR (character) data for the Nintendo Entertainment System (NES).

## Core Purpose

The primary function of this tool is to enable users to edit the 8x8 pixel graphical tiles (CHR data) used for sprites and background elements in NES games.

## Key Features

### 📁 File Handling
* **Load Files:**
    * NES ROMs (`.nes`) - CHR data is extracted.
    * CHR data files (`.chr`).
    * ZIP archives (`.zip`) - Auto-detects `.nes` or `.chr` files within.
* **Export Format:**
    * CHR File (`.chr`) - Standard NES character data (typically 8KB).
    * PNG Image (`.png`) - Exports the tile data as a 256x256 pixel image. (This likely means the 256 tiles from the CHR overview are arranged, perhaps as a 16x16 grid, with each 8x8 tile rendered as 16x16 pixels in the PNG to achieve the 256x256 dimension).
* **Clear:** Clears the current CHR data.

### 🎨 Editing Interface & Tools
* **CHR Overview (256 tiles):**
    * Displays a grid of 256 CHR tiles (likely one 4KB pattern table).
    * Users click on this grid (left panel) to select a tile for editing.
    * `Selected Tile`: Shows the index (e.g., 0) and hexadecimal value (e.g., 0x00) of the current tile.
    * `Position`: Shows the X, Y coordinates of the selected tile within the overview grid.
* **8x8 Tile Editor:**
    * A dedicated area (middle panel) where users can click to edit individual pixels of the selected 8x8 tile.
* **16x16 Metatile Preview:**
    * Shows a preview of how multiple 8x8 tiles (likely the selected tile and its neighbors, or a user-defined group) can combine to form a larger 16x16 "metatile."
* **Color Palette & Selection:**
    * Users choose a color by clicking color buttons or pressing `0-3` keys.
    * The palette consists of:
        * `0 (Black)`: Background/transparent
        * `1 (Dark Gray)`: Shadow/outline
        * `2 (Light Gray)`: Midtone/highlight
        * `3 (White)`: Brightest highlight
* **Editing Operations:**
    * `Undo`: `Ctrl+Z`
    * `Redo`: `Ctrl+Shift+Z` (or `Ctrl+Y` in some conventions)
    * `Copy Tile`: `Ctrl+C` (copies the current tile)
    * `Paste Tile`: `Ctrl+V` (pastes the copied tile)

### 📖 User Assistance
* **Help Menu:**
    * `User Manual`
    * `Basic Usage`
* **Status Information:**
    * Displays messages like "CHR Editor Ready - Please load a file".
    * Shows current mouse coordinates (e.g., `Mouse: (325, 132)`).

## 💾 Supported File Formats Summary

* **CHR:** Standard NES character data (8KB for a full bank, often 256 tiles per pattern table).
* **NES:** Complete ROM file (CHR data is extracted from it).
* **PNG:** Export format for a visual representation of the tiles (256x256 pixel image).
* **ZIP:** Archive format that can contain `.nes` or `.chr` files for easier loading.

## ⌨️ Keyboard Shortcuts

* `Ctrl+Z`: Undo
* `Ctrl+Shift+Z` (or `Ctrl+Y`): Redo
* `Ctrl+C`: Copy current tile
* `Ctrl+V`: Paste tile
* `0-3`: Select color from the palette

## 🎯 Intended Use

This editor is suitable for:
* NES homebrew game development.
* ROM hacking (modifying graphics in existing NES games).
* Pixel artists interested in creating graphics under NES limitations.

This appears to be a comprehensive and user-friendly tool for NES CHR manipulation.
