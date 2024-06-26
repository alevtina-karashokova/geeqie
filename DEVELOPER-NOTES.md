# Additional Information for Developers

## Non-standard icons

### Overlay Screen Display icons

#### ![][image_ref_image_osd_color_png] IMAGE_OSD_COLOR

#### ![][image_ref_image_osd_first_png] IMAGE_OSD_FIRST

#### ![][image_ref_image_osd_icon_png] IMAGE_OSD_ICON

#### ![][image_ref_image_osd_last_png] IMAGE_OSD_LAST

#### ![][image_ref_image_osd_rotate_auto_png] IMAGE_OSD_ROTATE_AUTO

Shown in the Overlay Screen Display. Defined in `./src/image-overlay.cc image_osd_icon_pixbuf()`.

## Menus

Menu processing is in `./src/layout-util.cc menu_entries[]`.

## File operation overrides

The standard copy, move, rename, delete and folder create functions can
be overridden by special plugins. The following defines are in `typedefs.h`:

```c
#define CMD_COPY     "geeqie-copy-command.desktop"
#define CMD_MOVE     "geeqie-move-command.desktop"
#define CMD_RENAME   "geeqie-rename-command.desktop"
#define CMD_DELETE   "geeqie-delete-command.desktop"
#define CMD_FOLDER   "geeqie-folder-command.desktop"
```

## Doxygen Documentation

Complete code documentation in html format can be generated via the script `./scripts/doxygen.sh`.

From the top level generated documentation, `Files / File List / scripts` provides a summary of files that may be useful.

[image_ref_image_osd_color_png]:
data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAC8AAAA4CAMAAABaKlG9AAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAaVBMVEUAAAAMDAwlJSUyMjJwcHCWlpbIyMjIu7vIoqLIlpbIV1fIMjLIAAC7opaiVzKWMgCiu5ZXojIylgCWyJYyyDIAyACWu6IyolcAljKWorsyV6IAMpaWlsgyMsgAAMiioshXV8i7u8j///+Wu6iCAAAAAWJLR0QiXWVcrAAAAAd0SU1FB+cMCxA4MY8D9CsAAAAQY2FOdgAAAGAAAABNAAAAEgAAAAaBW3h1AAAAiUlEQVRIx+3WwRaCIBSE4StIgqRpmqZB6Pu/ZMu7a8Ad5/Ct//0MUe4qIaOJikjUKlotiKS6RVPyWt9oA+mGe91aqNXcG3uHrCl9rn3XP6C+434Yn9A4cD/NL2ieSp9rv6xvaF243/YPtG/cO/+FvCt9rn04PHQE7s/goHBe39OUPvUPpP6N4p8ff3aBez1VWm4AAAAldEVYdGRhdGU6Y3JlYXRlADIwMjMtMTItMTFUMTY6NTY6MzcrMDA6MDAHcncUAAAAJXRFWHRkYXRlOm1vZGlmeQAyMDIzLTEyLTExVDE2OjQ2OjEzKzAwOjAwAcszBgAAAABJRU5ErkJggg==

[image_ref_image_osd_icon_png]:
data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADEAAAA3CAAAAACArv3dAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAAmJLR0QA/4ePzL8AAAAHdElNRQfnDAsQHzbLotPtAAAAEGNhTnYAAACxAAAAwgAAAC0AAACFGwGBxQAAAIhJREFUSMftlsENgCAQBEfDEwqgACzANqjXBizAAqAACoACfPhFc5roA7n3TrJ7l2wO2phBWyMW51RAWT+JibBEUGaa5Y5WYLydQ5365SRhlUhLBJyXEyVuAKXq6n6OTnSiE+0T1S7RDsBpOWH90XBywlzVfe/dN4lWbv7JrnKQi0PmySfz39kB1uwlKlcOPpIAAAAldEVYdGRhdGU6Y3JlYXRlADIwMjMtMTItMTFUMTY6MzA6NDQrMDA6MDDZ9N6UAAAAJXRFWHRkYXRlOm1vZGlmeQAyMDIzLTEyLTExVDE2OjMwOjQ0KzAwOjAwqKlmKAAAAABJRU5ErkJggg==

[image_ref_image_osd_rotate_auto_png]:
data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADEAAAA1CAAAAADNZlzWAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAAmJLR0QA/4ePzL8AAAAHdElNRQfnDAsRBQsiJQ8QAAAAEGNhTnYAAABCAAAASgAAAAkAAAAHVi99BwAAAPZJREFUSMfdlsENwyAMRX8rjjCAB0gGYA3mZYEO0AFgAAaAAXpooibBAlNVVRSfebzYsZ0A14ibJiM+nFMBFLlZTAQfAWVmK3+iB4D7cB7/IFSrMuDq2CCShxsjSszEWJp5JO/TiAMoEbWlUyvGotoEY+m+j8qigKUnqwiZtaj3PZEhclotyR2JEp/yXER9tcvlp534CXKWOOI48WsFNVm7mWy1vWk/8WGp4M6wI6qJfzAGQR4HQ5eoDF2iMnQIxtAhGEOT0BMss2EbBDkQhgjDL/1z7t2rEAoA9AQAk5YT5AoATXLCyD/pp61VDvLDIeObP5lzxgsCJ0kQ/qcmPwAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMy0xMi0xMVQxNzowMjo1NCswMDowMFXfsbMAAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjMtMTItMTFUMTY6NDU6MjMrMDA6MDBkc4/mAAAAAElFTkSuQmCC

[image_ref_image_osd_first_png]:
data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADEAAAAyCAAAAADQY2xuAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAAmJLR0QA/4ePzL8AAAAHdElNRQfnDAsRAzW1HrU9AAAAEGNhTnYAAABCAAAARQAAAAkAAAAFZ5jT+gAAAOhJREFUSMftls3NwyAMQF8rH8kADJAO0DUyLwt0gAwQBvAAZIAeKvpDTSA9fOon1acg8/RswFJgbxycH7o3J11B/HTqJpYQQYbTub+iC3Dc3Yfc62vEvV8B0BCbxDg9E2uc29XkMvb38ReEGKdB0rVY2cTj9pcQi5VN5NtPWjgvtapyaJgVNOhkvtE3Iuk8R2CNeKx3Lbbh9mVaxDZQt0jNULVIzfCwbBGvhmzZrmpoD/0L4af3yXI+bhAdhm+djx/xI/4rIQBuBBidvaXICuT5dt4miqxAa76L7Ad9pKV/85L45E/mO+MK4dVZDcfYdcQAAAAldEVYdGRhdGU6Y3JlYXRlADIwMjMtMTItMTFUMTc6MDI6MzgrMDA6MDBUENJAAAAAJXRFWHRkYXRlOm1vZGlmeQAyMDIzLTEyLTExVDE2OjQ3OjE3KzAwOjAwGkZ8KwAAAABJRU5ErkJggg==

[image_ref_image_osd_last_png]:
data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADcAAAA0CAAAAAALJP80AAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAAmJLR0QA/4ePzL8AAAAHdElNRQfnDAsRBCsAUB6ZAAAAEGNhTnYAAABDAAAASAAAAAIAAAAH0p+9FQAAAPFJREFUSMftlsERhCAMRf/ueIQCUgAWYBvUawMWsAVIARQgBexBF0USYdyD44y5AT4e0YAA94gXACjS1cDkAwA0AEC2rebG3kVOt139CgcAwPtkfk26binTbDRyvncAjOW5bDRywX0AIPDLykbP5vdwD/dw13HNvmM5H5NQVObmkyQNY8tcbmRsTH5kLZV6OJ/W8NgYFXUd8xdg3mc6P2tj89saBZvw/VaHYGN9q1G0ifUye0Rb5pvGtB2WIhinY873w28Gv28dccHJrZr8inHZ/lOm/LBROUc2FLnNjoqcrr8y/Z3fvkqOYqmcs/e6u8QXzO5OXKNeeskAAAAldEVYdGRhdGU6Y3JlYXRlADIwMjMtMTItMTFUMTc6MDM6MTMrMDA6MDD78Or5AAAAJXRFWHRkYXRlOm1vZGlmeQAyMDIzLTEyLTExVDE2OjQ3OjU5KzAwOjAwzjMJjAAAAABJRU5ErkJggg==
