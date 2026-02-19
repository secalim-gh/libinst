# libinst
Simple Bash Script to install local libraries.  
Useful for STB-Style (like stb.h) libs.

## Use
Looks for files on "~/.local/share/libinst/"  

```sh
libinst coro # searches for coro.* and copies first occurrence in PWD
libinst coro.h # searches explicitly for coro.h
libinst coro.h src/ # installs into PWD/src/
```

## Options
```sh
libinst --update
```
Looks for git repos, and updates them with git pull.  
  
```sh
libinst --add user/repo
```
Clones the provided repo and adds it to the installable libs.  
i.e. secalim-gh/coro gets expanded to  
https://github.com/secalim-gh/coro.git

