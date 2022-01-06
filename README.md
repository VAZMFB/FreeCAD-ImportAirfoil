# FreeCAD ImportAirfoil Macro ([FreeCAD-UveziAeroprofil](https://github.com/VAZMFB/FreeCAD-UveziAeroprofil) na Engleskom)

<p align="center">
  <img src="https://vazmfb.com/web/img/github/UveziAeroprofil.svg" width="150">
</p>

FreeCAD Macro for Airfoil coordinates import. It is possible, using simple dialog, to scale the airfoil, rotate, translate in the plane, translate along the span, select the plane and the main axis, as well as turn the geometry into a sketch. It is possible to import coordinates saved in the most commonly used formats.

Airfoil import is based on: https://github.com/VAZMFB/Python-importAirfoil

<p align="center">
  <img src="https://vazmfb.com/web/img/github/ImportAirfoil.png" width="800">
</p>

## Requirements
[FreeCAD](https://www.freecadweb.org/)<br>

Provided macro is tested with **FreeCAD 0.19**.

## Manual installation
If the **Addon Manager** is not used, the macro can be installed manually.

* Copy the Python code from the corresponding macro page.
* Open the macros menu `[Macro/Macros]`, press `[Create]`, and give it a name.
* Paste the Python code that you copied.
* Press the `[Save]` button, and restart FreeCAD.
* To use it, open again the macros menu, select your new macro, and press `[Execute]`.

## Notes for trailing edge

An open spline (type BSpline) is formed. Each airfoil is processed in order to open the geometry at the trailing edge and then close the geometry at that point with a straight line (TEdge). The aim of this modification is to obtain a single surface of the upper and lower part. Only one surface that is closed at the point of trailing edge with another surface is needed (otherwise the surface may be divided by the leading edge, which is not suitable for further finite element analysis).

## Usage

Run the macro program and follow the instructions.

## License
Copyright (C) 2021 Miloš Petrašinović <info@vazmfb.com>
 
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as 
published by the Free Software Foundation, either version 3 of the 
License, or (at your option) any later version.
  
This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.
  
You should have received a copy of the GNU General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
