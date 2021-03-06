# vdisp
#### *A virtual display implementation by ruby and curses*

<a href='https://i.gyazo.com/fbd5db8826c83cfe0b2b2263eb28ba07.png'>
  <img src='https://i.gyazo.com/fbd5db8826c83cfe0b2b2263eb28ba07.png' width='640' />
</a>

## Goals

- Make CUI splendid
- Show a lot of information
- Light-weight and fast

## Required environment
I checked operations by using the following ruby versions...

- Ruby 2.2.3 (My development environment)
- It may be available on other versions(which can use curses).

## How to use
### Download
Clone this project;

```
$ git clone https://github.com/rk0der/vdisp.git
```

### Launch
After that, in the directory you cloned to,

```
$ bin/vdisp
```

or use pipe

```
$ (other program) | bin/vdisp
```

You may want to get a log, then please add an option, -d or --debug.

```
$ bin/vdisp -d
```

At the version of 0.1.0, the program outputs the information to display.log.
You may be able to specify a filename by future implements.

### Internal command
At the version of 0.2.0 or newer, you can use the following commands after
launching program.

- /p [y] [x] [character/string]

Put a character or string on a specified position (y, x).
For example,

```
/p 1 1 Hello
```

- /pane [name] [y] [x] [height] [width] [material]

Create a pane
For example,

```
/pane pane0 0 0 20 20 *
```

- update

Refresh the screen.(normaly unneeded)

- /end

Terminate.

## Details
For more information, please visit [wiki](https://github.com/rk0der/vdisp/wiki).

## The Author
vdisp was started to develop by Ryota Kota(rk0der), a CS student
in Iwate Prefectural University, in 2015.

Welcome your contribution.

<ryo.alter@gmail.com>
