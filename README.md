# Cernak-lab-interactive-map
```mermaid
graph TD
    subgraph "Room A: Synthesis & HTE"
        GLV[Glovebox Station] --> |Status: Active| GL_LOG[Trouble Report/SOP]
        OP[Opentrons Robotics] --> |Status: Maintenance| OP_LOG[Trouble Report/SOP]
        SL[Schlenk Lines] --> |Status: Active| SL_LOG[Trouble Report/SOP]
    end

    subgraph "Room B: Analytical Core"
        GC[GC-MS: Metabolomics] --> |Status: Active| GC_LOG[Trouble Report/SOP]
        LC[UPLC-MS] --> |Status: Active| LC_LOG[Trouble Report/SOP]
        NMR[1D/2D NMR] --> |Status: Active| NMR_LOG[Trouble Report/SOP]
    end

    subgraph "Computational Zone"
        SYN[SYNTHIA / Cheminformatics] --> |Status: Active| SYN_LOG[Trouble Report/SOP]
    end

    %% Clickable Links to your .md files
    click GL_LOG "/logs/glovebox.md" "View History"
    click OP_LOG "/logs/opentrons.md" "Report Issue"
    click GC_LOG "/logs/gcms.md" "Find Solutions"
    click SYN_LOG "/logs/synthia.md" "Access Manual"

block-beta
  columns 4
  subgraph Room_A: "Synthesis Room"
    columns 2
    Glovebox:2
    Opentrons Schlenk_Line
  end
  subgraph Room_B: "Analysis"
    columns 1
    GC_MS
    NMR
  end
  Space:2
  Computer_Station:2
```
