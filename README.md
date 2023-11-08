![](https://github.com/senselogic/ATLAS/blob/master/LOGO/atlas.png)

# Atlas

Notion-like navigation plugin for Obsidian.

## Description

This plugin dynamically adds a parent note list and a child note list around the note title, so you can :

*   Quickly navigate up and down through the note hierarchy directly from the reading view.
*   Reveal the current note in the folder view through a dedicated icon.
*   Create parent folder notes by simply clicking on them in the list.
*   Create child notes through a dedicated icon or the "New child note" file menu option.

## Installation

*   In your vault folder, create a `.obsidian/plugins/atlas` subfolder.
*   Copy `main.js`, `manifest.json` and `styles.css` inside this subfolder.
*   Enable the Atlas plugin from the `Community plugins` settings panel.

## Usage

This plugin is best used :

*   On a Notion vault converted with [Topaz](https://github.com/senselogic/TOPAZ) :
    ```sh
    topaz --fix-paths --fix-newlines --fix-video-links --fix-titles --fix-indexes NOTION_EXPORT_FOLDER/ OBSIDIAN_VAULT_FOLDER/
    ```
*   Along with the following companion plugins :
    *   Local Images Plus :
        *   Process all new markdown files : yes.
        *   Process all new attachments : yes.
        *   Use MD5 for new attachments : no.
        *   Preserve link captions : yes.
        *   Add original filename or Open file tag : no.
        *   Include : .*\.md
        *   How to write paths in tags : Relative to note.
        *   Folder to save new attachments : Next to note in the folder specified below.
        *   Media folder : ${notename)
        *   Move/delete/rename media folder : yes.
    *   Fast Image Cleaner :
        *   Deleted Attachment Destination : Move to System Trash.
    *   At Symbol Linking :
        *   Include @ symbol : no.

## Limitations

*   The folder note must have the same name as its folder.
*   The lists appear after the note content.
*   The new sort order is only applied when Obsidian is restarted.

## Version

1.0

## Author

Eric Pelzer (ecstatic.coder@gmail.com).

## License

This project is licensed under the GNU General Public License version 3.

See the [LICENSE.md](LICENSE.md) file for details.

