# Awesome Mobile Graphics

A curated list of various learning resources for computer graphics on mobile devices.

- [Fundamental](#fundamental)
- [Best Practices](#best-practices)
  - [OpenGL ES](#opengl-es)
  - [Vulkan](#vulkan)
  - [Arm Mali](#arm-mali)
  - [Qualcomm Adreno](#qualcomm-adreno)
  - [Imagination PowerVR](#imagination-powervr)
  - [Apple](#apple)
- [Conferences](#conferences)
- [Sample Code](#sample-code)
  - [OpenGL ES](#opengl-es-1)
  - [Vulkan](#vulkan-1)
- [Profiling & Debugging](#profiling--debugging)
  - [Android](#android)
  - [Mali](#mali)
  - [Adreno](#adreno)
  - [Unreal](#unreal)
  - [Unity](#unity)

# Fundamental

* [GPU Framebuffer Memory: Understanding Tiling](https://developer.samsung.com/game/gpu-framebuffer) - A clear explanation with step-by-step animation.
* [Tile-based Rendering](https://developer.arm.com/solutions/graphics-and-gaming/developer-guides/learn-the-basics/tile-based-rendering/single-page) - A concise introduction to different rendering architectures with brief comparative analysis.
* [Mobile GPU Approaches to Power Efficiency](https://www.highperformancegraphics.org/wp-content/uploads/2019/hot3d/mobile_gpu_power_and_performance.pdf) by Andrew Gruber - An overview of power efficiency in terms of memory system, render pipeline, etc.

# Best Practices

* [Game Asset Optimizations](https://developer.samsung.com/game/asset) - Informative tips for app deployment and run-time performance.
* [Geometry Best Practices](https://developer.arm.com/solutions/graphics-and-gaming/developer-guides/game-artist-guides/geometry-best-practices/single-page) - Tips to strike a balance between geometry complexity and visual quality with lots of illustrations.
* [Textures Best Practices](https://developer.arm.com/solutions/graphics-and-gaming/developer-guides/game-artist-guides/texture-best-practices/single-page) - A number of texturing tips help apps run smoother and look better.
* [Understanding Numerical Precision](https://developer.arm.com/solutions/graphics-and-gaming/developer-guides/learn-the-basics/understanding-numerical-precision/single-page) - A brief guide to properly choose numerical precision and to preserve accuracy of the numbers.
* [Cramming Software onto Mobile GPUs](https://community.arm.com/cfs-file/__key/communityserver-blogs-components-weblogfiles/00-00-00-20-66/siggraph2015_2D00_mmg_2D00_andrew_2D00_slides.ppt) by Andrew Garrard - Various essential techniques to well utilize mobile hardware.

## OpenGL ES

* [OpenGL ES Usage Recommendations](https://developer.samsung.com/game/opengl) - Practical and effective tips for GLES programming.
* [How to Correctly Handle Framebuffers](https://community.arm.com/developer/tools-software/graphics/b/blog/posts/mali-performance-2-how-to-correctly-handle-framebuffers) by Peter Harris - A crystal clear explanation with sample code for avoiding redundant tile writes.

## Vulkan

* [Vulkan Usage Recommendations](https://developer.samsung.com/game/usage) - Effective guidelines for Vulkan API.
* [Introduction to Vulkan Render Passes](https://developer.samsung.com/game/renderpasses) - A detailed note about how to use render passes in Vulkan API.
* [Getting Faster and Leaner on Mobile: Optimizing Roblox with Vulkan](https://robloxtechblog.com/getting-faster-and-leaner-on-mobile-optimizing-roblox-with-vulkan-7c79950fef69) by Arseny Kapoulkine - Informative optimization experiences with several concrete examples.

## Arm Mali

* [Graphics and Gaming Development](https://developer.arm.com/solutions/graphics-and-gaming) - Official Mali developer resources.
* [Arm Mali GPU Best Practices Developer Guide](https://developer.arm.com/documentation/101897/latest) - A complete guide for Mali graphics programming with OpenGL ES and Vulkan.
* [Mali GPU OpenGL ES 3.x Developer Guide](https://developer.arm.com/documentation/100587/0100/introduction) - An introductory guide for Pixel Local Storage, ASTC, and other 3.x features.
* [Understanding Render Passes](https://developer.arm.com/documentation/102479/0100) - Practical guides for efficient render passes with Vulkan and OpenGL ES.
* [The Benefits of Buffer Packing](https://developer.arm.com/solutions/graphics-and-gaming/developer-guides/learn-the-basics/the-benefits-of-buffer-packing/single-page) - Several performance tips related to bandwidth usage saving.

## Qualcomm Adreno

* [Game Developer Guides.](https://developer.qualcomm.com/docs/adreno-gpu/developer-guide/gpu/gpu.html)

## Imagination PowerVR

* [Architecture Guides.](https://github.com/powervr-graphics/Native_SDK/tree/master/docs/Architecture%20Guides)


## Apple

* [Metal video learning resources.](https://developer.apple.com/videos/graphics-and-games/metal)
* [Modern Rendering with Metal](https://developer.apple.com/videos/play/wwdc2019/601/) - Demonstration of how to apply Metal features to implement deferred and tiled-forward rendering.
<!-- * [Ray Tracing with Metal](https://developer.apple.com/videos/play/wwdc2019/613/) -->

# Conferences

* [Moving Mobile Graphics,](https://community.arm.com/graphics/b/blog/posts/moving-mobile-graphics) SIGGRAPH Course Notes - Technical and inspirational talks from practitioners at the forefront.
  * Video recording: [2020,](https://www.youtube.com/watch?v=wOBCWZJq6zs) [2018,](https://dl.acm.org/doi/10.1145/3214834.3214857) [2016,](https://dl.acm.org/doi/10.1145/2897826.2927312) [2015.](https://dl.acm.org/doi/10.1145/2776880.2787664)
* [Event Archive from Galaxy GameDev](https://developer.samsung.com/galaxy-gamedev/event-archive.html) - Quite a few collected slides and videos from conference talks at GDC, Unreal Summit, Unity Unite, etc.

# Sample Code

## OpenGL ES

* [Mali OpenGL ES SDK for Android.](https://github.com/ARM-software/opengl-es-sdk-for-android)
* [Adreno SDK for OpenGL ES.](https://developer.qualcomm.com/docs/adreno-gpu/developer-guide/components/asdkgles.html)

## Vulkan

* [Vulkan Samples](https://github.com/KhronosGroup/Vulkan-Samples) - Educational source code with informative explanation for developing optimized Vulkan application.
* [Android Vulkan Tutorial](https://github.com/googlesamples/android-vulkan-tutorials) - Beginner guide to develop Vulkan sample with Android Studio.

# Profiling & Debugging

* [RenderDoc](https://renderdoc.org/) ([video tutorials](https://youtube.com/playlist?list=PLWziqE5d25dXo1IE150YJiPT9EIW8ymta)) - A lightweight, reliable and developer friendly debugger for quick frame diagnosis.
* [Principles of High Performance](https://developer.arm.com/solutions/graphics-and-gaming/developer-guides/learn-the-basics/principles-of-high-performance/single-page) - Core ideas for mobile app optimization.
* [Optimization checklist](https://developer.arm.com/documentation/dui0555/b/optimization-checklist/the-checklist?lang=en) - A handy checklist for common performance bottlenecks.

## Android

* [Android GPU Inspector](https://gpuinspector.dev/) - A unified profiler for various GPU IP on Android.
* [Perfetto](https://perfetto.dev/docs/) - An open-source stack for system profiling, app tracing and trace analysis.

## Mali
* [Arm Mobile Studio](https://developer.arm.com/tools-and-software/graphics-and-gaming/arm-mobile-studio) ([video tutorial](https://www.youtube.com/watch?v=gcxIuwBZyic)) - A developer suite contains graphics analyzer, GPU profiler and performance advisor.
* [Android performance triage with Streamline](https://developer.arm.com/tools-and-software/graphics-and-gaming/arm-mobile-studio/learn/tutorials/android-performance-triage-with-streamline) - A step-by-step diagnosis guide to identify performance problem.
* [Accelerating Mali GPU analysis using Streamline](https://community.arm.com/developer/tools-software/graphics/b/blog/posts/accelerating-mali-gpu-analysis-using-arm-mobile-studio) by Peter Harris - A quick overview of using Streamline template charts.
* [Workload Pipelining](https://developer.arm.com/solutions/graphics-and-gaming/developer-guides/learn-the-basics/workload-pipelining/single-page) - A clear illustration of various pipeline bottlenecks.
* [Frame Pipelining](https://community.arm.com/developer/tools-software/graphics/b/blog/posts/the-mali-gpu-an-abstract-machine-part-1---frame-pipelining) by Peter Harris - A lucid explanation of   asynchronous execution of rendering pipeline beneath GL APIs.
* [Mali GPU Performance Counters.](https://developer.arm.com/ip-products/graphics-and-multimedia/mali-gpus/mali-performance-counters)
* [Mali GPU Datasheet.](https://developer.arm.com/solutions/graphics-and-gaming)

## Adreno

* [Snapdragon Profiler.](https://developer.qualcomm.com/software/snapdragon-profiler)
* [Available functionality for supported texture format.](https://developer.qualcomm.com/docs/adreno-gpu/developer-guide/gpu/spec_sheets.html#texture-formats)

## Unreal

* [Profiling and Optimization in UE4](https://www.youtube.com/watch?v=EbXakIuZPFo) by Paulo Souza - An introductory tutorial for identifying performance problems.
* [UE4 Performance and Profiling](https://www.youtube.com/watch?v=hcxetY8g_fs) by Zak Parrish - Comprehensive guidelines for optimization process.
* [UE4 Graphics Profiling](https://www.youtube.com/playlist?list=PLF8ktr3i-U4A7vuQ6TXPr3f-bhmy6xM3S) by Tech Art Aid - A well organized and informative tutorial series for beginners.

## Unity

* [Introduction to profiling in Unity](https://www.youtube.com/watch?v=uXRURWwabF4) by Ciro Continisio - A beginner tutorial on CPU profiler and frame debugger.
* [Tackling profiling for mobile games with Unity and Arm](https://blogs.unity3d.com/2021/03/11/tackling-profiling-for-mobile-games-with-unity-and-arm/) by Mark Harkness - A crisp introduction to mobile game optimization with various tools.
* [Better Together: Integrating Arm Mobile Studio with Unity](https://community.arm.com/developer/tools-software/graphics/b/blog/posts/integrating-arm-mobile-studio-with-unity) by Geraint North - A concrete example of how Streamline annotations make better data interpretation.
