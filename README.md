DWANGO OpenToonz плагины ([日本語](./README_ja.md))
=================

Этот репозиторий содержит пример плагинов для разработчиков.
Эти плагины зависят от [opentoonz_plugin_utility](https://github.com/opentoonz/opentoonz_plugin_utility).
Которые требуют OpenCV3 runtime. [Visual C++ Redistributable Packages для Visual Studio 2013](https://www.microsoft.com/en-US/download/details.aspx?id=40784) is also required on Windows.

## Как использовать готовые плагины

[osx](https://github.com/opentoonz/dwango_opentoonz_plugins/releases/download/v1.0.0/dwango_opentoonz_plugins_osx.zip) и [win](https://github.com/opentoonz/dwango_opentoonz_plugins/releases/download/v1.0.0/dwango_opentoonz_plugins_win.zip) are zip archives which contain prebuilt plugins.
Вы можете установить их с помощью следующих шагов:

0. Скопируйте файлы `.plugin` , которые вы хотите, в `${path-to-opentoonz-stuff}/plugins/`.
  - `${path-to-opentoonz-stuff}` это `/Applications/OpenToonz/OpenToonz_1.0_stuff/plugins/` (OSX) или `C:\OpenToonz 1.0 stuff\plugins` (Windows) by default.
0. Установите `OpenCV3`.
0. Перезапустите OpenToonz.

Руководство поплагину [здесь](./doc/sample_plugins_manual.md).

### Как установить OpenCV3

#### OSX

Вы можете установить `OpenCV3` с помощью `homebrew`.

```
brew install opencv3
brew ln opencv3 --force
```

#### Windows

0. Скачайте [OpenCV для Windows VERSION 3.1](http://opencv.org/).
0. Установите переменную окружения `PATH` в `${path-to-opencv3}\build\x64\vc12\bin\`,  
  - или скопируйте `${path-to-opencv3}\build\x64\vc12\bin\opencv_world310.dll` в `C:\Program Files\OpenToonz 1.0`. 
