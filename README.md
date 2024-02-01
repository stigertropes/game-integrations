changes from original

- genshin
    -   gimi addon (see notes below)
    -   added fps unlock addon (144 fps since no per-game/per-addon settings)
    -   enable vkbasalt with env (since no per-game env)

- star rail
    -   srmi addon (see notes below)
    -   enable vkbasalt with env (since no per-game env)

#### gimi/srmi notes

gimi and srmi require additional d3d dlls

download and extract `https://github.com/lutris/d3d_extras/releases/latest`

copy all files from x64 folder to system32 (`anime-games-launcher/components/prefix/drive_c/windows/system32`)

copy all files from x32 folder to syswow64 (`anime-games-launcher/components/prefix/drive_c/windows/syswow64`)

open wine user.reg (`anime-games-launcher/components/prefix/user.reg`)

find `[Software\\Wine\\DllOverrides]`

add following lines there
```
"d3dcompiler_33"="native"
"d3dcompiler_34"="native"
"d3dcompiler_35"="native"
"d3dcompiler_36"="native"
"d3dcompiler_37"="native"
"d3dcompiler_38"="native"
"d3dcompiler_39"="native"
"d3dcompiler_40"="native"
"d3dcompiler_41"="native"
"d3dcompiler_42"="native"
"d3dcompiler_43"="native"
"d3dcompiler_46"="native"
"d3dcompiler_47"="native"
"d3dx10"="native"
"d3dx10_33"="native"
"d3dx10_34"="native"
"d3dx10_35"="native"
"d3dx10_36"="native"
"d3dx10_37"="native"
"d3dx10_38"="native"
"d3dx10_39"="native"
"d3dx10_40"="native"
"d3dx10_41"="native"
"d3dx10_42"="native"
"d3dx10_43"="native"
"d3dx11_42"="native"
"d3dx11_43"="native"
"d3dx9_24"="native"
"d3dx9_25"="native"
"d3dx9_26"="native"
"d3dx9_27"="native"
"d3dx9_28"="native"
"d3dx9_29"="native"
"d3dx9_30"="native"
"d3dx9_31"="native"
"d3dx9_32"="native"
"d3dx9_33"="native"
"d3dx9_34"="native"
"d3dx9_35"="native"
"d3dx9_36"="native"
"d3dx9_37"="native"
"d3dx9_38"="native"
"d3dx9_39"="native"
"d3dx9_40"="native"
"d3dx9_41"="native"
"d3dx9_42"="native"
"d3dx9_43"="native"
```

#### srmi notes

the new loader doesn't work with wine

as a workaround download the v1.0 version of srmi, extract and move `W11Loader.exe` to srmi addon folder (`anime-games-launcher/games/star-rail/global/addons/extra/srmi/3dmigoto`)
 

# Original README

# Anime Games Launcher integrations scripts index

Index of games integrations scripts for the [anime games launcher](https://github.com/an-anime-team/anime-games-launcher). Documentation can be found in [here](https://github.com/an-anime-team/anime-games-launcher/blob/master/GAMES_INTEGRATION.md).
