# hyprbars

Adds simple title bars to windows.

![preview](https://i.ibb.co/GkDTL4Q/20230228-23h20m36s-grim.png)

## Config

All config options are in `plugin:hyprbars`:

```
plugin {
    hyprbars {
        # config
        # exludes non floating windows and windows that have one of these titles Easy Effects|Volume Control|Bluetooth|iwgtk
        exclude_windowrulev2 = floating:0,title:^(Easy Effects|Volume Control|Bluetooth|iwgtk)$
        buttons {
            # button config
        }
    }
}
```

`bar_color` -> (col) bar's background color

`bar_height` -> (int) bar's height (default 15)

`col.text` -> (col) bar's title text color

`bar_text_size` -> (int) bar's title text font size (default 10)

`bar_text_font` -> (str) bar's title text font (default "Sans")

`exclude_windowrulev2` -> like hyprland windowrulev2 `WINDOW` filter. currenly if any conditon in the rule is met the window will be ignored.


## Buttons Config

`button_size` -> (int) the size of the buttons.

`col.maximize` -> (col) maximize button color

`col.close` -> (col) close button color
