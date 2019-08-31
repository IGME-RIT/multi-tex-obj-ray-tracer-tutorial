Documentation Author: Niko Procopi 2019

This tutorial was designed for Visual Studio 2017 / 2019
If the solution does not compile, retarget the solution
to a different version of the Windows SDK. If you do not
have any version of the Windows SDK, it can be installed
from the Visual Studio Installer Tool

Welcome to the Ray Tracing Multi-Texture Tutorial!
Prerequesites: 
	Ray Tracing Textures
	Anisotropic Filtering

We make an array of uniforms for the textures
We make a meshID that goes with each triangle, which is assigned
in the compute shader before going to the fragment shader, then the
fragment shader uses the meshID in each triangle to choose which
texture is rendered. In main.cpp, each texture is assigned to each
mesh, right before glDrawArrays