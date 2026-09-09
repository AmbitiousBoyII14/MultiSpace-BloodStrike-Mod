# MultiSpace-BloodStrike-Mod

Multi Space host app with the BloodStrike **ModMenu (ImGui)** baked in — rootless mod. Clone BloodStrike inside Multi Space and the menu appears in-game.

## Download

Grab the APK from **[Releases](../../releases)** (or the `MultiSpace-BloodStrike-Mod.apk` file in this repo).

## Build info

- Host: Multi Space 1.1.3 (`com.dualspace.multispace.android`), clean base + patched loader
- Menu: ImGui ModMenu, touch via `MotionEvent::copyFrom` hook in `libinput.so`
- Native payload: `lib/arm64-v8a/libbsmenu.so`
- Patch offset intact: `0x471e320`
- Signed (installs over previous copies of this mod)

## Install

1. Download the APK from Releases
2. Install it (installs over the previous copy — same signing key, no need to uninstall)
3. Open Multi Space, clone/import BloodStrike, launch it from inside Multi Space
4. Menu should appear — tap/drag to test touch

Built from source commit `a044d69` (v1.3: key system + white UI).
