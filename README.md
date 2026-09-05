# Taskbar Count Badges

![Taskbar Count Badges examples](images/showcase.png)

**Current release:** 1.1.0

Taskbar Count Badges shows how many windows are represented by each app button on the Windows 11 taskbar using customizable number badges or compact dots.

## What's New in 1.1

- Added top and bottom dot positions
- Top and bottom dots are displayed horizontally
- Bottom dots replace the native Windows running indicator and show from one running window
- Left, right, and top dot positions keep the native Windows running indicator unchanged
- Windows task progress indicators remain untouched
- Improved bottom-dot indicator handling and cleanup

## Display Styles

### Number Badge

Shows the number of windows represented by each taskbar app button.

The badge can be customized with:

- Circle, rounded-square, or square shape
- Badge size and position
- Horizontal and vertical offsets
- Background, text, and border colors
- Border thickness
- Font family, size, and weight
- Configurable maximum number, with larger values shown using `+`

### Dots

Shows a minimal stack or row of dots around the app icon.

- Left and right positions use a vertical stack
- Top and bottom positions use a horizontal row
- Bottom replaces the native Windows running indicator
- Bottom shows one dot for one running window
- Left, right, and top leave the native Windows running indicator unchanged
- Windows task progress indicators remain untouched
- Configurable dot size and color
- Up to five dots are shown; five dots means five or more windows

## Settings

![Taskbar Count Badges settings](images/settings.png)

### Display

Choose between:

- Number badge
- Dots

### Number Badge

Configure:

- Shape
- Size
- Position
- Horizontal and vertical offsets
- Background color
- Text color
- Border color
- Border thickness
- Font family
- Font size
- Font weight
- Maximum displayed count

### Dots

Configure:

- Left, right, top, or bottom position
- Dot size
- Dot color

## Behavior

By default, no count indicator is shown when a taskbar button represents a single window. The indicator appears when that button represents two or more windows.

The minimum window count can be changed in the settings.

Bottom dots are the exception: they always start at one window because they replace the native Windows running indicator.

Window counts update automatically as windows are opened and closed, and settings are applied live.

## Compatibility

- Windows 11 only
- Supports x64 and ARM64 Windows
- Works with multiple monitors and secondary Windows taskbars

On multi-monitor systems, the count follows each individual taskbar button. Depending on the Windows multi-monitor taskbar configuration, the same app can therefore show different counts on different monitors. Moving a window between monitors can change the count shown on each taskbar.

The mod is designed primarily for grouped or combined taskbar app buttons. When taskbar buttons are configured to stay uncombined, Windows can expose multiple buttons for the same app group, so the same app count may appear on more than one button.

Third-party taskbar replacements or tools that replace the native Windows 11 taskbar may not be compatible.

## Notes

Taskbar Count Badges uses the taskbar's own per-button grouping information instead of independently scanning all desktop windows. Counts therefore follow Windows taskbar grouping, including per-taskbar behavior on multi-monitor systems.

The indicators are visual only and do not change taskbar grouping, combining, window ordering, application behavior, or task progress.

## License

GPL-3.0
