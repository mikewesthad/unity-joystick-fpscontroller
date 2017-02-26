# unity-joystick-fpscontroller

A package for my Unity classes - a modified version of the Unity FPS controllers that works with the Xbox 360 controller (and other joysticks).

# Details

This package is a modification of the standard asset first-person characters so that they play nicely with controllers. The modifications are:

1. Run button uses virtual axis for input, so that it can be configured in the Input Manager.
1. Run button is modified to either be controlled by: holding the button to run or using the button to toggle between run & walk.
1. Mobile/touch controls are dropped.

The virtual axes (in Input Manager) that the controllers use:

    Horizonal & Vertical - movement
    Mouse X & Mouse Y - looking
    Jump
    Run

Define those in the input manager (Project Settings -> Input) in order set up the controls. The default setup in Unity:

    Horizonal & Vertical - arrow keys or WASD keys
    Mouse X & Mouse Y - mouse movement
    Jump - spacebar
    Run - not assigned

An Xbox 360-compatible InputManager.asset setup is included in this package that has the following controls:

    Horizonal & Vertical - left stick or arrow keys or WASD keys
    Mouse X & Mouse Y - right stick or mouse movement
    Jump - "a" button or spacebar
    Run - press left stick or shift

To use that InputManager:

1. Close Unity and open up your project folder in explorer/finder.
1. Make a backup of ProjectSettings/InputManager.asset (in case you want to go back to your previous setup).
1. Replace ProjectSettings/InputManager.asset with the InputManager.asset in this package.
1. Boot up Unity!
