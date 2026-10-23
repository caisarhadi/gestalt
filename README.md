# Gestalt with the OFB26 project

This repository hands out a built Gestalt with the OFB26 project, so the OFB26 shader timeline can be worked on without building Gestalt. The download holds no source code and no footage.

Gestalt is in an experimental state, earlier than an alpha release. It is handed out for the OFB26 shader timeline and the render of the OFB26 shader, which work in this build.

## Download

Download `Gestalt-OFB26-2026-10-23.zip` from this repository's Releases page (release `ofb26-2026-10-23`).

## Requirements

- Windows 10 or Windows 11, 64-bit.
- An NVIDIA RTX GPU. The build was run on a GeForce RTX 5090 with driver 616.92.
- A drive `D:`. Gestalt and the project are made for the folder `D:\CPM_Claude\Gestalt`. A machine without a drive `D:` can make one from any folder with `subst D: C:\GestaltDrive` in a command prompt.

## Install

Extract the zip to `D:\`. The files then stand in `D:\CPM_Claude\Gestalt`:

- `bin\gestalt\Gestalt.exe` and its runtime, the Visual C++ runtime included.
- `library`, which holds the shaders; the OFB26 shaders are `library\examples\shaders\ofb26_BrandTakeover` and `library\examples\shaders\ofb26_BrandTakeover_Var02`.
- `assets`.
- `state\gestalt\projects\OFB26`: the project file `OFB26.gestalt`, its timelines and the After Effects projects of the six looks.

## Open the OFB26 shader timeline

1. Start `D:\CPM_Claude\Gestalt\bin\gestalt\Gestalt.exe`.
2. Choose File > Open Project… and open `D:\CPM_Claude\Gestalt\state\gestalt\projects\OFB26\OFB26.gestalt`.
3. Open the timeline `OFB26_ShaderPlates` (6:30 at 30 fps). Its track Video 1 holds the six looks of the shader `ofb26_BrandTakeover`: ORBITAL VIEW (look 0), MORNING FOREST (look 1), UNDERWATER (look 2), ROLLING FIELDS (look 3), EV FOREST (look 4) and CRYSTALLINE (look 5).

The delivery timelines `100_AIWHE_RedwoodsAM-Loop-A` to `152_AIWHE_Earth-Loop-C` also use footage, which is not in the download; their footage clips show as offline.

## Build

The build is Gestalt of 23 October 2026 (commit `76dfe50b` of `caisarhadi/CPM_Claude`, built at 18:28), with the Blur effect's Repeat Edge Pixels; the project and the shaders are those of the same commit.
