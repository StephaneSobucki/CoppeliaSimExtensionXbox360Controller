# CoppeliaSim Xbox360 Controller plugin

This project is a fork from https://github.com/horothesun/VREPExtensionXbox360Controller.
I just replaced a few lines of code to make it compatible with CoppeliaSim.

## How to build (Skip this part if you want to use the pre-compiled dll)

1. git clone https://github.com/StephaneSobucki/CoppeliaSimExtensionXbox360Controller
2. mkdir build
3. cd build
4. cmake ..

Then open xbox\_controller.sln in Visual Studio. Either right-click on "ALL\_BUILD" in the solution explorer then select build or press ctrl+shift+b simultaneously

The resulting shared library simExtXbox360Controller.dll is found in the Debug folder

## How to use in CoppeliaSim

First, you need to put the dll file in the root folder of CoppeliaSim.
To check if the plugin was successfully loaded, in the Menu bar click on Tools and then select User Settings. In the floating window that just opened untick "Hide console window". In the console, you can check if the plugin was successfully loaded. It should say "Plugin 'Xbox360Controller': load succeeded."

I also included an example CoppeliaSim scene (based on the controlledViaScript scene) to show how the plugin works.
