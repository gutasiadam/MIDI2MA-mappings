
# MIDI2MA-mappings

**MA Macros for allowing MIDI controllers to control parts of grandMA2 onPC software using the software's Remote Input.**
## How to use the repo
Folder names are named after a specific midi controller (eg. Novation Launchpad MK2). In it, you can find various macros for various mappings (like an onPC keyboard mapping). Every mapping macro has a *Layout.pdf* file included with it, showing what part of the controller is mapped to what command wing part.

folder structure structure looks like this:

    CONTROLLERNAME
	    - Layout.pdf
	    - commandWingKeyboard
		    - Layout.pdf
		    - CONTROLLERNAME_commandWingKeyboard.xml
		- commandWingFaderController
			- Layout.pdf
			-  CONTROLLERNAME_commandWingFaderController.xml
	CONTROLLER2NAME
		- commandWingKeybaord
			- Layout.pdf
			- CONTROLLER2NAME_commandWingKeybaord.xml
    
where *CONTROLLERNAME* is the MIDI controller's name (like the Novation Lauchpad MK2), *commandWingKeyboard* is the name of the macro (and what it does), Layout.pdf is a schematic of the controller from which is clear what the mapped buttons do, and *CONTROLLERNAME_commandWingKeyboard.xm*l is the actual MACRO file itself.
## How to contribute
If you made a mapping macro for a MIDI controller that isn't listed in the repo, feel free to contribute it to this repository.

### How can I add my contribution to the repo?
A submission works by creating a pull request, adding the following files to the repo:

- If there is no folder for your MIDI controller, create one first (`CONTROLLERNAME`) .
- Folder name should be the name of the Macro (`Whatitdoes`) 
 - [ ] The MA macro file itself. It should be named `CONTROLLERNAME_Whatitdoes.xml`
	 - Please add a brief description to the beginning of the XML file:
		 - The midi controller's name,
		 - What it does, (how it works)
		 - (optionally with the date created, a description, and your name)
 - [ ] A layout file, from which is clear, what is mapped to what in MA named `Layout.pdf`.
 - [ ] *(optional)* Any other file (e.g images for a color picker macro) that you feel is necessary for your macro to work effectively.

## A macro doesn't work as it's Layout states, what should I do?
- If you fixed the Macro yourself, please create a pull request with the corrected files.
- Optionally, **open an issue** with the controller and the macro's name. Describe your issue and select a corresponding label.



