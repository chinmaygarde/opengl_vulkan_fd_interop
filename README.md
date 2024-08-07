# OpenGL Vulkan Interop

Demonstrates how to perform interop between OpenGL and Vulkan via the `VK_KHR_external_memory` (Vulkan),  `GL_EXT_memory_object` (OpenGL ES) and related extensions.

This was prototyped for [Impeller](https://github.com/flutter/engine/tree/9932f34aac4e81d95fa17e06134038ca6472a0e4/impeller#readme) for the Flutter Engine. The need was to do this on Android and a reliable way to do this on that platform was to use Android Hardware Buffers instead. On Android, the FD based extensions are only available on a subset of devices.

So, this implementation was ripped out and [replaced with one that uses Android Hardware Buffers](https://github.com/flutter/engine/pull/53966).

This repository contains that now defunct implementation for posterity and in case the need for this arises again in the future.
