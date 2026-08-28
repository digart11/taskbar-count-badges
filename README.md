# Taskbar Count Badges

See how many windows are represented by each app button on the Windows 11 taskbar.

Taskbar Count Badges adds a small customizable indicator when a taskbar app
button represents multiple windows. The indicator can be shown as either a
**number badge** or compact **dots**.

## Screenshots

### Customization examples

![Taskbar Count Badges examples](https://raw.githubusercontent.com/digart11/taskbar-count-badges/main/images/showcase.png)

### Settings

![Taskbar Count Badges settings](https://raw.githubusercontent.com/digart11/taskbar-count-badges/main/images/settings.png)

## Display styles

### Number badge

Shows the number of windows represented by that taskbar button.

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
- Windows task progress indicators are left untouched
- Change dot size and color
- Up to five dots are shown; five dots means **five or more windows**

## Behavior

By default, no count indicator is shown when a taskbar button represents a
single window. The indicator appears when that button represents two or more
windows.

The minimum window count can be changed in the settings.

Bottom dots are the exception: they always start at one window because they
replace the Windows running indicator.

Window counts update automatically as windows are opened and closed, and
settings are applied live.

## Compatibility

- Windows 11 only
- Supports x64 and ARM64 Windows
- Works with multiple monitors and secondary Windows taskbars

On multi-monitor systems, the count follows each individual taskbar button.
Depending on the Windows multi-monitor taskbar configuration, the same app can
therefore show different counts on different monitors. Moving a window between
monitors can change the count shown on each taskbar.

The mod is designed primarily for grouped/combined taskbar app buttons. When
taskbar buttons are configured to stay uncombined, Windows can expose multiple
buttons for the same app group, so the same app count may appear on more than
one button.

Third-party taskbar replacements or tools that replace the native Windows 11
taskbar may not be compatible.

## Notes

The mod uses the taskbar's own per-button grouping information instead of
independently scanning all desktop windows. Counts therefore follow Windows
taskbar grouping, including per-taskbar behavior on multi-monitor systems.

The indicators are visual only and don't change taskbar grouping, combining,
window ordering, application behavior, or task progress.