# Bonsai.AlliedVision
[Bonsai](http://www.open-ephys.org/bonsai/) library containing modules for acquiring images from Allied Vision cameras that use the [Vimba SDK](https://www.alliedvision.com/en/products/software.html).

## Installation
The NuGet package for this library can be found in Bonsai's package manager. It is available at [MyGet](https://www.myget.org/feed/bonsai-community/package/nuget/Bonsai.AlliedVision) and the [NuGet Gallery](https://www.nuget.org/packages/Bonsai.AlliedVision/).

Alternatively, you can install this from a local package by adding the .nuget folder to Bonsai's package manager (more information can be found [here](https://bonsai-rx.org/docs/packages/)).

## Usage
After the NuGet package is added to Bonsai, a **VimbaCapture** source node will become available. This node will produce a sequence of frames captured from a connected Allied Vision camera that uses the Vimba SDK.

### Important Note:
Due to the way that the Vimba.NET dll is written, running the **VimbaCapture** node will currently cause Bonsai to crash unless it is launched with an additional flag:

`Bonsai.exe --noboot`
