# practice-time-reviewer

A portable desktop application for batch reviewing audio recordings and manually auditing verified playing time using a DAW-style waveform interface with exportable reports.

---

## Overview

**practice-time-reviewer** is an offline desktop workstation designed for educators and moderators who need to review large volumes of student audio recordings and produce defensible measurements of actual playing time.

The tool is intentionally **manual-first**:
- No automatic detection
- No AI-based timing
- No background monitoring

All counted time is explicitly marked by the reviewer. This prioritises accuracy, transparency, and auditability over convenience.

---

## Key Features

- **Batch moderation**
  - Drag-and-drop multiple audio files into a queue
  - Continuous playback across files
  - Resume exactly where you left off

- **DAW-style waveform interface**
  - Zoomable waveform with playhead and time ruler
  - Keyboard-first transport controls
  - Precise region marking

- **Manual time marking**
  - Spacebar toggles counted playing regions on/off
  - Multiple regions per file
  - Per-region assignment to students (for ensemble recordings)

- **Multi-student support**
  - Maintain a roster for a review session
  - Assign regions to different students within the same recording
  - Per-student totals across a batch

- **Auditability**
  - Per-file review records saved alongside audio
  - File hash verification to detect tampering
  - Draft / Final states with optional locking
  - Change history for region edits

- **Exports for administration**
  - Batch summary CSV (per student totals)
  - Per-region audit CSV
  - Optional PDF reports for record-keeping

- **Offline & portable**
  - No network access required
  - Runs without admin privileges
  - Portable EXE distribution (Windows)

- **Modern UI**
  - Light / Dark / System theme
  - Dockable panels
  - Keyboard shortcut overlay

---

## What This Tool Is (and Isn’t)

### This tool **is**
- A review workstation for converting recordings into verified playing-time records  
- Designed for compliance, moderation, and administrative workflows  
- Built for speed, repeatability, and audit trails  

### This tool **is not**
- An automated practice detector  
- An AI judge of performance quality  
- A background monitoring or surveillance tool  
- A music player or DAW for creative work  

All time measurements come from explicit human marking.

---

## Typical Workflow

1. Drag multiple recordings into the batch queue.
2. Press play.
3. Press **Space** to start counting when playing begins.
4. Press **Space** again to stop counting when playing stops.
5. Repeat for each playing section.
6. Assign regions to students if multiple students appear in one recording.
7. Review totals and validation warnings.
8. Finalise and export reports.

---

## Keyboard Shortcuts (Default)

- **Enter** – Play / Pause  
- **Space** – Toggle counted region (start/stop)  
- **J / L** – Seek −2s / +2s  
- **Shift + J / Shift + L** – Seek −10s / +10s  
- **[ / ]** – Playback speed down / up  
- **Backspace** – Undo last mark  
- **Ctrl + Z / Ctrl + Y** – Undo / Redo  
- **N / P** – Next / Previous file in batch  

Contains:
- Audio file hash
- Marked regions
- Student assignments
- Totals and status (Draft/Final)
- Audit log

### Batch session index

Tracks:
- Queue state
- Progress across files
- Roster and settings

---

## Supported Audio Formats

- WAV  
- MP3  

(Additional formats supported if built with FFmpeg.)

---

## Installation

No installer required.

1. Download the latest portable release.
2. Extract the ZIP archive.
3. Run `practice-time-reviewer.exe`.

The application stores settings and cache files in user space and does not require administrator privileges.

---

## Data & Privacy

- All processing is local.
- No network access is required or used.
- No microphone access is required.
- Review data is stored alongside audio files or in the user profile directory.
- No telemetry or analytics are collected.

---

## Project Status

This project is under active development.  
The interface and file formats may evolve before a stable release.

---

## Contributing

Contributions are welcome.  
Please open an issue to discuss significant changes before submitting a pull request.

---

## License

Specify your license here (e.g., MIT, GPL-3.0, Apache-2.0).

---

## Disclaimer

This tool measures playing time based solely on reviewer-marked intervals.  
It does not claim to objectively measure practice quality or completeness.  
All outputs should be interpreted in the context of your institution’s policies.
---

## File Formats

### Review file (saved next to each audio file)
