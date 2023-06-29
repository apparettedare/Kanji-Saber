# 漢字セイバーのセットアップ

漢字セイバーのセットアップ方法を記述します．

## Unityのインストール
[ここ](https://unity.com/ja/download)からUnityをインストール．  
OSとUnityのバージョンは以下の通りです．  
| 番号 | アイテム       | 説明    |
|:--:| ---------- |----------------|
| 1  | OS         | Windows10    |
| 2  | Unity      | [Unity 2020.3.26f1](https://unity.com/releases/editor/whats-new/2020.3.26) |

## 漢字セイバープロジェクトの作成方法  

1. Open this project with Unity.
1. Click [**Ignore**] in the [Enter Safe Mode?] window.
1. Click [Assets]-[Import Package]-[Custom Package...].
1. Select a common unitypackage (e.g. robocup-common.unitypackage) and open the file.
1. Click [Import] button.
1. Click [Assets]-[**Reimport All**].
1. Click [**Reimport**] button.
1. Please confirm that no error occurred in Console window.


### VOICE VOXのインストール

If you want to output speech, please do the following two steps.

#### Windows Settings
Please install the English language if you are using other than English.  
The procedure is like as follows.
1. Open the Windows settings menu
2. Click [Time & Language] - [Region & language]
3. Click [Add a language] in [Languages]-[Preferred languages]
4. Select "English (United States)" and Install

#### Import Files
Please import files by following the steps below.
1. Prepare "ConsoleSimpleTTS.exe" and "Interop.SpeechLib.dll".  
For details on these files, see [here](https://github.com/RoboCupatHomeSim/console-simple-tts).
2. Copy those files to the "TTS" folder in the same directory as SIGVerseConfig folder.


### Build
1. Create a "Build" folder under this project folder.
1. Open this project with Unity.
1. Click [File]-[Build Settings].
1. Click [Build]
1. Select the "Build" folder , and type a file name (e.g. Handyman) and save the file.
1. Copy the "TTS" folder under the "Build" folder.

## How to Set Up

### Modify Configuration

1. Open this project with Unity.
2. Click [SIGVerse]-[SIGVerse Settings].  
SIGVerse window will be opened.
3. Type the IP address of ROS to "Rosbridge IP" in SIGVerse window.

## How to Execute Handyman

Please start the ROS side application beforehand.  
See [handyman-ros](https://github.com/RoboCupatHomeSim/handyman-ros) for an example application.

### Execute on Unity Editor
1. Click [SIGVerse]-[Set Default GameView Size].
2. Double click "Assets/Competition/Handyman/Handyman(.unity)" in Project window.
3. Click the Play button at the top of the Unity editor.

### Execute the Executable file
1. Double Click the "Handyman.exe" in the "Build" folder.

## License

This project is licensed under the SIGVerse License - see the LICENSE.txt file for details.
