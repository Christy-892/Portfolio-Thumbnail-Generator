# Portfolio-Thumbnail-Generator
## Overview
An investigation into Unreal Engine’s UMG (Unreal Motion Graphics), focused on developing a portfolio thumbnail generator capable of producing consistent thumbnails while maintaining a cohesive visual style and structure over time. The project initially began as an in-game UI system before later being transitioned into an **Editor Utility**. This shift provided a far more practical workflow, enabling thumbnails to be created efficiently and exported directly as .png files

---
## User Guide
1. Ensure you have added any images you wish to use in the "MainImage_Images" folder:
<img width="800" height="500" alt="image" src="https://github.com/user-attachments/assets/d5d30da2-ebfc-43cb-9af1-c68ed78f9067" /><br>

2. In the **Content Browser**, navigate to the "EU_PortfolioThumbnail" **Editor Utility Widget** and _RMB>Run Editor Utility Widget_:
<img width="800" height="500" alt="image" src="https://github.com/user-attachments/assets/6ac1830c-e5cc-477b-8891-4d8c1e9d659d" /><br>

3. Make any alterations needed:<br>
<img width="800" height="500" alt="image" src="https://github.com/user-attachments/assets/dd1034d8-30c6-4a16-b1b4-4ae0e3b88433" /><br>

4. Select "Save Image":<br>
<img width="800" height="500" alt="image" src="https://github.com/user-attachments/assets/f515768b-fb38-423c-9045-475565713c7a" /><br>

---
## Features
### Drag/Drop Icon Control
The drag/drop icon control allows for an intuitive approach to selecting and placing the icons:<br>
<img width="1280" height="720" alt="Feature_DragDrop" src="https://github.com/user-attachments/assets/01fac6fe-b422-4298-8a9e-a035a551e48b" /><br>


### Main Image Control
Options to alter the image size and position:<br>
<img width="1280" height="720" alt="Feature_MainImageControl" src="https://github.com/user-attachments/assets/7504da45-9ae3-496d-94c0-348e059f5628" /><br>

---
## Deep Dive
### Editor Utility Widget
The Editor Utility Widget was setup with 2 custom Widget Blueprints. The left side is the "Editor Panel", and the right side is the "Preview Panel":<br>
<img width="800" height="500" alt="Editor Utility Designer" src="https://github.com/user-attachments/assets/6390c433-d2c5-4056-8d5d-954acbfec4fc" />

There is very little logic on these individual blueprints, with the majority of logic happening in the Editor Utility graph:<br>
<img width="800" height="500" alt="Editor Utility Graph" src="https://github.com/user-attachments/assets/4b04b768-2344-4ee6-818e-1bd2f826e937" />


### Drag/Drop Icon Control

### Render Target
---
## Setup
>[!NOTE]
> - Unreal Engine version - 5.7.3

1. Download the file from this repository
2. Copy the folder "PortfolioThumbnailGenerator" into your Unreal Engine projects "Contents/UI" folder **via explorer**

## Resources
- Great drag/drop inventory tutorial - https://www.youtube.com/watch?v=m39FbAA_u7s
- Artstation Portfolio Piece - https://www.artstation.com/artwork/mAJgm9

## To Do
- [x] Proof Of Concept
- [x] Convert from in-game UI to Editor Utility
- [x] Feature - Drag/Drop icon control
- [x] Feature - Main image selection control
- [x] Feature - Main image size/position control
- [x] Feature - Custom Name and Folder input
- [ ] Improvement - Drag/Drop to swap icons if dropped on valid icon
- [ ] Improvement - Ensure only one instance can be present at a time
