# Geneva Cross Mechanism for an Intermittent Conveyor

A mechanical-design project: a Geneva drive (Maltese cross) that turns a continuous motor rotation into the stop-and-go motion a conveyor needs to hold a product at a station and then release it.

**What it shows:** kinematic design in SolidWorks (parts, sub-assemblies, mates), a generated Blender scene that animates the mechanism from a Python script, a state-of-the-art literature review with checked sources, and a short pitch video.

## Stack
- SolidWorks 2025: parts, assemblies, and the conveyor sub-assembly
- Blender 4.2 with a Python generator (`bpy`) for the animated scene
- STL meshes for 3D printing
- Literature review in PDF and HTML

## Structure
| Folder | Contents |
|---|---|
| `02_DOCUMENTO/` | State-of-the-art review and bibliography (PDF, HTML) |
| `03_PIEZAS_STL/` | Nine mesh parts (flywheel, pin, cross, cam, crank, shafts) |
| `04_SOLIDWORKS/` | Native part and assembly files |
| `05_BLENDER/` | Blender project and the Python scene generator |
| `06_CAPTURAS/` | Seven 1920x1080 screenshots of the mechanism |
| `07_RENDERS/` | Short MP4 clips used in the pitch |

Not included: `01_VIDEO/VIDEO_PITCH_CRUZ_GINEBRA.mp4` (53 MB, over the 20 MB limit for this repository).

## How to run
- SolidWorks: open the part files first, then `Ensamblaje1.SLDASM`.
- Blender: open `05_BLENDER/GENEVA_CONVEYOR_PROJECT.blend`, or regenerate the scene with `blender -b --python 05_BLENDER/geneva_conveyor_generator.py -- --mode build`.

## Honest status
- Built for a university mechanisms course. The assembly and the Blender scene were not re-run in this staging pass.
- The STL files are imported meshes without feature history, so they are for printing or visual reference, not for editing parametric features.
- The author states every bibliography entry has a verifiable link or DOI; some publisher pages may require institutional access.
---

> **Consolidated project.** This repository also replaces the former `geneva-drive-mechanism` (identical assets, archived).
