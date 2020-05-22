# MicroShell
Mirror of CuBeatSystems MicroShell https://cubeatsystems.com/microshell/  
Copyright (C) 2016-2017 Shinichiro Nakamura (CuBeatSystems)

## What's this?
Have you tried to develop a key input feature on your small embedded platform with a serial input? It is not so easy to implement correctly because the input methodology is using a complicated protocol known as VT100. In my recent project "Natural Tiny Shell (NT-Shell)" provides VT100 compatible terminal control features for small embedded systems. However, the middleware is still large for small embedded processors such as 8-bit MCUs, 16-bit MCUs and also for small 32-bit MCUs like Cortex-M0. This "MicroShell" middleware provides a minimal terminal control for the platforms.

## Features

* Compatible with VT100 :)
* Really simple.
  * The API of the microshell module has only two functions.
  * It consists of only two small modules in the core layer.
* Highly portable.
  * Compatible with C89.
  * No dependencies. (even libc!)
  * No dynamic memory allocation. (no need a operating system!)
* Small code foot print.
  * ROM: Less than 5.0KB
  * RAM: Less than 0.5KB

## Edit Controls

Action | Key input
------ | ---------
Move to the start of line 	|CTRL+A or Home
Move to the end of line 	|CTRL+E or End
Move forward one character 	|CTRL+F or Right arrow
Move back one character 	|CTRL+B or Left arrow
Delete previous character 	|Backspace
Delete current character 	|CTRL+D or Delete
Cancel current input line 	|CTRL+C 