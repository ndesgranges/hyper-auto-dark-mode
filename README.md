# Description

This plugin will set your terminal to use the Atom One Light theme in the day and Atom One Dark theme at night.

> This is is a fork from [johnviolano/hyper-day-night-switch](https://github.com/johnviolano/hyper-day-night-switch) repository which does not exist anymore. See  [[npm] hyper-day-night-switch](https://www.npmjs.com/package/hyper-day-night-switch)
>
> The goal of this fork is to provide an "auto" behavior that relies on system dark mode settings instead of manually setting the hour

# Install

Edit ~/.hyper.js and include the plugin name:

```
module.exports = {
    config: {
        plugins: ['hyper-day-night-switch'],
    }
}
```

# Config

Not setting these ends up setting the plugin in "auto" mode. It will try to replicate the system dark/light hours.

```
module.exports = {
    config: {
        dayNightSwitch: {
            sunUp: 6,
            sunDown: 21
        },
    }
}
```

# Themes

These are the themes this plugin will use:

```
hyper-one-light
hyperterm-atom-dark
```


# TODO
- [ ] MacOS : get current theme (dark/light)
- [ ] Windows : get current theme (dark/light)
- [ ] Linux : get current theme (dark/light)