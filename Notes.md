# Notes on Program Structure

## Installation

Following OS X instructions on https://github.com/mxgmn/WaveFunctionCollapse/issues/3

Unable to install via

```bash
$ brew install mono (if you don't have it)
WaveFunctionCollapse $ mcs -pkg:dotnet /reference:System.Drawing.dll *.cs
WaveFunctionCollapse $ mono Main.exe
```

Works after following `dzoba`'s instructions:

```
$ brew cask install mono-mdk
$ open /usr/local/Caskroom/mono-mdk/4.6.1.3/MonoFramework-MDK-4.6.1.3.macos10.xamarin.universal.pkg
$ env PATH=/Library/Frameworks/Mono.framework/Commands/:$PATH mcs -pkg:dotnet /reference:System.Drawing.dll *.cs
$ env PATH=/Library/Frameworks/Mono.framework/Commands/:$PATH mono Main.exe
```

Output of the above is

```
< Chess
> DONE
> DONE
< Chess
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
< City
> DONE
> DONE
< Flowers
> DONE
> DONE
< Hogs
> DONE
> DONE
< Hogs
> CONTRADICTION
> DONE
> CONTRADICTION
> DONE
< Knot
> DONE
> CONTRADICTION
> DONE
< Less Rooms
> DONE
> DONE
< Mountains
> DONE
> DONE
< Office
> DONE
> DONE
< Paths
> DONE
> DONE
< Platformer
> DONE
> DONE
< Platformer
> DONE
> DONE
< Red Maze
> DONE
> DONE
< Rooms
> DONE
> CONTRADICTION
> DONE
> DONE
< Rule 126
> DONE
> DONE
< Simple Knot
> DONE
> DONE
< Simple Maze
> DONE
> DONE
< Simple Wall
> DONE
> DONE
< Simple Wall
> DONE
> DONE
< Simple Wall
> DONE
> DONE
< Simple Wall
> DONE
> DONE
< Trick Knot
> DONE
> DONE
< Village
> DONE
> DONE
< Water
> DONE
> DONE
< Summer
> DONE
> DONE
< Castle
> CONTRADICTION
> DONE
> DONE
< Circuit
> DONE
> DONE
> DONE
< Knots
> DONE
> DONE
< Knots
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> DONE
> CONTRADICTION
> CONTRADICTION
> DONE
< Knots
> DONE
> DONE
< Knots
> DONE
> DONE
< Knots
> DONE
> DONE
< Knots
> DONE
> DONE
< Knots
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> CONTRADICTION
> DONE
< Knots
> DONE
> DONE
< Knots
> DONE
> DONE
< Knots
> DONE
> DONE
< Rooms
> DONE
> DONE
< Circles
> DONE
> DONE
< Circles
> DONE
> DONE
< Circles
> DONE
> DONE
< Circles
> DONE
> DONE
< Village
> DONE
> DONE
< Summer
> DONE
> DONE
< 3Bricks
> DONE
> CONTRADICTION
> DONE
```

Program generated a bunch of PNGs in the current directory for ones that succeeded.

## Questions

What is the difference between the Overlapping and the Simple Tiled models?

Why are there multiple copies of variables that are just the image width and height? Why `FMX`, `FMY`?
