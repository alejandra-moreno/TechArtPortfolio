# Batch Rename Tool  

## Why this tool?
When handling large scenes (hundreds of props, dozens of lights, etc) being able to batch rename assets quickly helps maintain naming conventions, enhances scene organization, and improves team collaboration while reducing possible errors. This tool provides a convenient UI inside the editor to select many objects and apply consistent renaming patterns (prefix/suffix, find/replace, numbering, etc). This small but useful utility reflects my interest in editor scripting, in-engine tooling, and streamlining art pipelines. 

## Key Features  
- Select multiple actors/assets from the World Outliner or Content Browser.  
- Define a rename pattern (e.g., `Enemy_{0}`, `Prop_Chair_{Suffix}`, etc).  
- Prefix, suffix, find & replace functionality.  
- Automatically increments numbers for a series.  
- Safe: preview changes before committing the rename.  
- Easily integrated into your editor workflow as a Utility Widget.

## Files Included

### `ActorAction_BatchRename`
*Editor Utility Blueprint*  
Handles batch-renaming operations for **actors** selected in the World Outliner.  
Provides logic for iterating through selected actors and applying the rename pattern.

### `AssetAction_BatchRename`
*Editor Utility Blueprint*  
Manages batch-renaming for **assets** selected in the Content Browser.  
Includes logic for safely renaming assets while preserving references.

### `EUW_BatchRename`
*Editor Utility Widget*  
The main **UI panel** for the Batch Rename Tool.  
Contains the rename input fields, preview list, and all user-facing interactions.

### `EUW_BatchRename_ListItem`
*Editor Utility Widget*  
A UI **list entry widget** used for previewing each item’s old name and new name before applying the rename operation.

## Screenshots & Demo  
See the `UsageExamples/` folder for before/after renaming and the UI in action.

## Installation & Usage  
1. Copy the `BatchRename/` folder contents into your Unreal project’s `Plugins/` or `EditorUtilityWidgets/` directory.  
2. In the Unreal Editor, go to *Window → Editor Utility Widgets* and open *Batch Rename Widget*.  
3. Select the actors/assets you wish to rename.  
4. Set your naming pattern, choose options (prefix, suffix, etc).  
5. Click *Preview* to see proposed names, then *Apply* to rename.  
6. (Optional) Script or assign shortcut for quicker access.

## License  
This project is licensed under the MIT License – see [LICENSE.md](LICENSE.md) for details.

## Contact  
Alejandra Moreno Grande · moreno.grande.alejandra@gmail.com · [CV](https://drive.google.com/drive/folders/1Psl4Bz29ofrFvHQg2aOiIuQzeiTZbPSr?usp=sharing) · [LinkedIn](http://www.linkedin.com/in/alejandra-moreno-grande-29b6a8220)

