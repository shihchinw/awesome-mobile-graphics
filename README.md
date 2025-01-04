# Awesome Mobile Graphics

A curated list of various learning resources for computer graphics on mobile devices.

- [Fundamentals](#fundamentals)
- [Best Practices](#best-practices)
  - [OpenGL ES](#opengl-es)
  - [Vulkan](#vulkan-1)
  - [Arm Mali](#arm-mali)
  - [Qualcomm Adreno](#qualcomm-adreno)
  - [Imagination PowerVR](#imagination-powervr)
  - [Apple](#apple)
- [Conferences](#conferences)
- [Sample Code](#sample-code)
  - [OpenGL ES](#opengl-es-1)
  - [Vulkan](#vulkan-2)
- [Profiling \& Debugging](#profiling--debugging)
  - [Vulkan](#vulkan-3)
  - [Android](#android)
  - [Mali](#mali)
  - [Adreno](#adreno)
  - [Unreal](#unreal)
  - [Unity](#unity)

# Fundamentals

* [GPU Framebuffer Memory: Understanding Tiling](https://developer.samsung.com/game/gpu-framebuffer) - A clear explanation with step-by-step animation.
* [Tile-based Rendering](https://developer.arm.com/solutions/graphics-and-gaming/developer-guides/learn-the-basics/tile-based-rendering/single-page) - A concise introduction to different rendering architectures with brief comparative analysis.
* [Mobile GPU Approaches to Power Efficiency](https://www.highperformancegraphics.org/wp-content/uploads/2019/hot3d/mobile_gpu_power_and_performance.pdf) by Andrew Gruber - An overview of power efficiency in terms of memory system, render pipeline, etc.

## Vulkan
* [Vulkan Tutorial](https://www.khronos.org/assets/uploads/developers/library/2016-vulkan-devu-seoul/1-Vulkan-Tutorial_English.pdf) by Hyokuen Lee, Minwook Kim - Instructive slides for rendering a textured quad from the ground up.
* [Introduction to Vulkan Render Passes](https://developer.samsung.com/game/renderpasses) - A detailed note about how to use render passes in Vulkan API.

# Best Practices

* [Game Asset Optimizations](https://developer.samsung.com/game/asset) - Informative tips for app deployment and run-time performance.
* [Geometry Best Practices](https://developer.arm.com/documentation/102448/0200) - Tips to strike a balance between geometry complexity and visual quality with lots of illustrations.
* [Textures Best Practices](https://developer.arm.com/documentation/102449/0200) - A number of texturing tips help apps run smoother and look better.
* [Optimizing Assets for Mobile VR](https://www.youtube.com/watch?v=3JCg62e9zdA) - General tips on game asset optimization for mobile platforms.
* [Understanding Numerical Precision](https://developer.arm.com/solutions/graphics-and-gaming/developer-guides/learn-the-basics/understanding-numerical-precision/single-page) - A brief guide to properly choose numerical precision and to preserve accuracy of the numbers.
* [Cramming Software onto Mobile GPUs](https://community.arm.com/cfs-file/__key/communityserver-blogs-components-weblogfiles/00-00-00-20-66/siggraph2015_2D00_mmg_2D00_andrew_2D00_slides.ppt) by Andrew Garrard - Various essential techniques to well utilize mobile hardware.

## OpenGL ES

* [OpenGL ES Usage Recommendations](https://developer.samsung.com/game/opengl) - Practical and effective tips for GLES programming.
* [How to Correctly Handle Framebuffers](https://community.arm.com/developer/tools-software/graphics/b/blog/posts/mali-performance-2-how-to-correctly-handle-framebuffers) by Peter Harris - A crystal clear explanation with sample code for avoiding redundant tile writes.

## Vulkan

* [Vulkan Usage Recommendations](https://developer.samsung.com/game/usage) - Effective guidelines for Vulkan API.
* [Vulkan FAQ for Mobile Developers.](https://arm-software.github.io/vulkan_best_practice_for_mobile_developers/docs/faq.html)
* [Vulkan Case Study](https://www.khronos.org/assets/uploads/developers/library/2016-vulkan-devu-seoul/2-Vulkan-Case-Study.pdf) by Soowan Park, Joonyong Park - Informative dev tips related to swapchain, uniform buffer and rendering.
  * [More experiments on uniform buffer management](https://youtu.be/y-EBiswp3qU?t=915) ([slides](https://www.khronos.org/assets/uploads/developers/library/2017-gdc/GDC_Vulkan-on-Mobile_Vulkan-Game-Development-in-Mobile-Samsung_Mar17.pdf)) by Soowan Park.
* [Vulkan Samples](https://github.com/KhronosGroup/Vulkan-Samples/blob/main/samples/README.adoc) - Comprehensive resources of case study and best practices.
  * [Surface Rotation](https://github.com/KhronosGroup/Vulkan-Samples/blob/main/samples/performance/surface_rotation/README.adoc) - How appropriately use surface rotation, which was handled transparently by OpenGL ES driver.
  * [Render passes](https://github.com/KhronosGroup/Vulkan-Samples/blob/main/samples/performance/render_passes/README.adoc) - How attachment load/store operations might affect performance.
  * [Subpasses](https://github.com/KhronosGroup/Vulkan-Samples/blob/main/samples/performance/subpasses/README.adoc) - How tile-based renderer might save bandwidth.
  * [Pipeline Barriers](https://github.com/KhronosGroup/Vulkan-Samples/blob/main/samples/performance/pipeline_barriers/README.adoc) - How efficiently set up pipeline barriers, with a focus on pipeline stages.
* [Getting Faster and Leaner on Mobile: Optimizing Roblox with Vulkan](https://medium.com/@zeuxcg/getting-faster-and-leaner-on-mobile-optimizing-roblox-with-vulkan-7c79950fef69) by Arseny Kapoulkine - Informative optimization experiences with several concrete examples.
  * Optimizing Roblox: Vulkan Best Practices for Mobile Developers ([slides](https://zeux.io/data/gdc2020_arm.pdf), [video](https://www.gdcvault.com/play/1026767/Optimizing-Roblox-Vulkan-Best-Practices)), GDC 2020.

## Arm Mali

* [Mali GPU Training](https://youtube.com/playlist?list=PLKjl7IFAwc4QUTejaX2vpIwXstbgf8Ik7) - A comprehensive training series from mobile graphics fundamentals to performance analysis.
* Mali Optimization Resources with [Unreal](https://www.arm.com/resources/unreal) and [Unity](https://www.arm.com/resources/unity) - Introductory guidelines for profiling games and optimizing artwork.
* [Graphics and Gaming Development](https://developer.arm.com/solutions/graphics-and-gaming) - Official Mali developer resources.
* [Arm Mali GPU Best Practices Developer Guide](https://developer.arm.com/documentation/101897/latest) - A complete guide for Mali graphics programming with OpenGL ES and Vulkan.
* [Mali GPU OpenGL ES 3.x Developer Guide](https://developer.arm.com/documentation/100587/0101/introduction) - An introductory guide for Pixel Local Storage, ASTC, and other 3.x features.
* [Understanding Render Passes](https://developer.arm.com/documentation/102479/0100) - Practical guides for efficient render passes with Vulkan and OpenGL ES.
* [The Benefits of Buffer Packing](https://developer.arm.com/solutions/graphics-and-gaming/developer-guides/learn-the-basics/the-benefits-of-buffer-packing/single-page) - Several performance tips related to bandwidth usage saving.
* [Using Asynchronous Compute on Arm Mali GPUs: A Practical Sample](https://community.arm.com/developer/tools-software/graphics/b/blog/posts/using-asynchronous-compute-on-arm-mali-gpus) by Hans-Kristian Arntzen - An informative introduction to async-compute scheduling on Mali devices.
* [Deferred Shading on Mobile: An API Overview](https://community.arm.com/developer/tools-software/graphics/b/blog/posts/deferred-shading-on-mobile) by Hans-Kristian Arntzen - A crisp introduction to bandwidth saving techniques on deferred shading with various API options.
* [Hidden Surface Removal in Immortalis-G925: The Fragment Prepass](https://community.arm.com/arm-community-blogs/b/graphics-gaming-and-vr-blog/posts/immortalis-g925-the-fragment-prepass) by Tord Øygard - An in-depth explanation on how Fragment Prepass works, along with best practices to avoid performance pitfalls.

## Qualcomm Adreno

* [Game Developer Guides](https://docs.qualcomm.com/bundle/publicresource/topics/80-78185-2/best_practices.html) - A best practice for Adreno graphics programming with OpenGL ES and Vulkan.
  * [Practical Shader Optimization Tips on Adreno Architectures.](https://docs.qualcomm.com/bundle/publicresource/topics/80-78185-2/best_practices.html#shaders-2)
* [OpenCL General Programming and Optimization Guide.](https://docs.qualcomm.com/bundle/publicresource/80-NB295-11_REV_C_Qualcomm_Snapdragon_Mobile_Platform_Opencl_General_Programming_and_Optimization.pdf)

## Imagination PowerVR

* [Developer Documentation](https://docs.imgtec.com/html/index.html)
* [Performance Recommendations](https://docs.imgtec.com/performance-guides/performance-recommendations/html/topics/introduction.html) - An informative recommendations range from high-level effect techniques to low-level GLSL optimization.

## Apple

* [Metal Video Learning Resources.](https://developer.apple.com/videos/graphics-games)
* [Modern Rendering with Metal](https://developer.apple.com/videos/play/wwdc2019/601/) - Demonstration of how to apply Metal features to implement deferred and tiled-forward rendering.
<!-- * [Ray Tracing with Metal](https://developer.apple.com/videos/play/wwdc2019/613/) -->

# Conferences

* [Moving Mobile Graphics,](https://community.arm.com/arm-community-blogs/b/graphics-gaming-and-vr-blog/posts/moving-mobile-graphics) SIGGRAPH Course Notes - Technical and inspirational talks from practitioners at the forefront.
  * Video recordings: [2020,](https://www.youtube.com/watch?v=wOBCWZJq6zs) [2018,](https://dl.acm.org/doi/10.1145/3214834.3214857) [2016,](https://dl.acm.org/doi/10.1145/2897826.2927312) [2015.](https://dl.acm.org/doi/10.1145/2776880.2787664)
* [Event Archive from Galaxy GameDev](https://developer.samsung.com/galaxy-gamedev/event-archive.html) - Quite a few collected slides and videos from conference talks at GDC, Unreal Summit, Unity Unite, etc.
* Vulkanised - Informative best and worst practices from game devs pioneering with Vulkan
  * Video recordings: [2024,](https://vulkan.org/events/vulkanised-2024) [2023,](https://vulkan.org/events/vulkanised-2023#talks) [2022,](https://www.khronos.org/events/vulkanised-webinar-february-2022) [2021,](https://www.khronos.org/events/vulkanised-2021) [2019,](https://www.khronos.org/developers/library/2019-vulkanised-is-back) [2017.](https://www.khronos.org/events/vulkanised-experience-from-game-devs-pioneering-with-vulkan1)

# Sample Code

## OpenGL ES

* [Mali OpenGL ES SDK for Android.](https://github.com/ARM-software/opengl-es-sdk-for-android)
* [Adreno SDK for OpenGL ES.](https://developer.qualcomm.com/software/adreno-gpu-sdk)
* [PowerVR OpenGL ES Examples.](https://github.com/powervr-graphics/Native_SDK/tree/master/examples/OpenGLES)

## Vulkan

* [Vulkan Samples](https://github.com/KhronosGroup/Vulkan-Samples) - Educational source code with informative explanation for developing optimized Vulkan application.
* [Android Vulkan Tutorial](https://github.com/googlesamples/android-vulkan-tutorials) - Beginner guide to develop Vulkan sample with Android Studio.
* [PowerVR Vulkan Examples.](https://github.com/powervr-graphics/Native_SDK/tree/master/examples/Vulkan)

# Profiling & Debugging

* [RenderDoc](https://renderdoc.org/) ([video tutorials](https://youtube.com/playlist?list=PLWziqE5d25dXo1IE150YJiPT9EIW8ymta)) - A lightweight, reliable and developer friendly debugger for quick frame diagnosis.
* [Principles of High Performance](https://developer.arm.com/solutions/graphics-and-gaming/developer-guides/learn-the-basics/principles-of-high-performance/single-page) - Core ideas for mobile app optimization.
* [Basic Optimization Checklist](https://developer.arm.com/documentation/101897/0301/Optimization-basics/Basic-optimization-checklist) - A handy checklist for common performance bottlenecks.

## Vulkan
* [Vulkan Ecosystem Developer Tools](https://www.youtube.com/watch?v=jItHShexBf4&t=14403s) ([slides](https://www.lunarg.com/wp-content/uploads/2023/05/Vulkan-Ecosystem-Developer-Tools-Osaka-MAY2023.pdf)) by Spencer Fricke - A quick roll call of available dev-tools to prevent reinventing the wheel.
* [Using Vulkan Validation Effectively](https://www.youtube.com/watch?v=jItHShexBf4&t=10224s) ([slides](https://www.lunarg.com/wp-content/uploads/2023/11/Using-Vulkan-Validation-Effectively-Osaka.pdf)) by Spencer Fricke - An instructive guide for using validation layer and debug utilities extension.
* [Introduction to Using SPIR-V](https://www.youtube.com/watch?v=jItHShexBf4&t=13229s) ([slides](https://www.lunarg.com/wp-content/uploads/2023/05/SPIRV-Osaka-MAY2023.pdf)) by Spencer Fricke - A quick start guide for learning how to read and understand SPIR-V.

## Android

* [Game Development Guides on Android,](https://developer.android.com/games/guides) including tools, libraries, best practices, etc.
* [Modern Android Development Skills on Performance](https://www.youtube.com/playlist?list=PLWz5rJ2EKKc-xjSI-rWn9SViXivBhQUnp) - A video series of brief overviews on various profiling tools (ex. Systrace, Perfetto, etc.) on Android.
* [Android GPU Inspector](https://developer.android.com/agi) - A unified profiler for various GPU IPs on Android (only for few [supported devices](https://developer.android.com/agi/supported-devices) currently).
  * [Analyze a System Trace](https://developer.android.com/agi/sys-trace/long) - A comprehensive tutorial of system inspection.
* [System Tracing](https://developer.android.com/topic/performance/tracing)
  * [Android Profiler](https://developer.android.google.cn/studio/profile/android-profiler) - Tools for inspecting usage of CPU, memory, network, and battery resources.
  * [Systrace for Games](https://www.youtube.com/watch?v=4oAlB-3tkqc) by Tim Murray - An introductory video tutorial with case studies.
  * [Improve Game Performance on Android](https://developer.android.com/games/optimize#improve-performance-areas) - Tips for identifying and improving various aspects of common performance concerns in mobile games.
* [Android Vulkan layers](https://solidpixel.github.io/2022/04/20/android_vulkan_layers.html) by Peter Harris - A quick recipe to get Vulkan validation layers working for Android applications.
* [Enable Vulkan Layers Outside the Application](https://developer.android.com/ndk/guides/graphics/validation-layer#enable-layers-outside-app) - Instructions for enabling layers with adb commands.
* [Enable Vulkan Debug Callback on Android](https://developer.android.com/ndk/guides/graphics/validation-layer#enable_the_debug_callback) - Example code snippets for enablement.
<!-- * [Perfetto](https://perfetto.dev/docs/) - An open-source stack for system profiling, app tracing and trace analysis. -->
<!-- * [Android Game Development Extension for Visual Studio](https://developer.android.com/games/agde/quickstart?hl=en) -->

## Mali
* [Arm Performance Studio](https://developer.arm.com/Tools%20and%20Software/Arm%20Performance%20Studio%20for%20Mobile) - A developer suite contains GPU profiler, frame analyzer, and offline shader compiler.
  * [Optimizing mobile games using Arm Mobile Studio](https://www.youtube.com/watch?v=gcxIuwBZyic) - A quick overview on performance optimization workflow.
  * Educational [videos](https://on-demand.arm.com/flow/arm/devhub/sessionCatalog/page/pubSessCatalog?search.category=1680252620842003scxY) and step-by-step [tutorials](https://learn.arm.com/learning-paths/smartphones-and-mobile/) on Arm Developer Hub.
* [Android performance triage with Streamline](https://developer.arm.com/documentation/102540/latest) - A step-by-step diagnosis guide to identify performance problem.
* [Accelerating Mali GPU analysis using Streamline](https://community.arm.com/developer/tools-software/graphics/b/blog/posts/accelerating-mali-gpu-analysis-using-arm-mobile-studio) by Peter Harris - A quick overview of using Streamline template charts.
* [Workload Pipelining](https://developer.arm.com/solutions/graphics-and-gaming/developer-guides/learn-the-basics/workload-pipelining/single-page) - A clear illustration of various pipeline bottlenecks.
* [Frame Pipelining](https://community.arm.com/developer/tools-software/graphics/b/blog/posts/the-mali-gpu-an-abstract-machine-part-1---frame-pipelining) by Peter Harris - A lucid explanation of asynchronous execution of rendering pipeline beneath GL APIs.
* Mali GPU Performance Counters: [Immortalis-G925/Mali-G725](https://developer.arm.com/documentation/109793/0101/Arm--Immortalis-G925-and-Mali-G725-GPU-performance-counters?lang=en), [G720](https://developer.arm.com/documentation/108081/0101/Arm--Immortalis-G720-and-Mali-G720-GPU-performance-counters?lang=en), [G715](https://developer.arm.com/documentation/107776/0100/?lang=en), [G710](https://developer.arm.com/documentation/102813/0102/?lang=en), and <a href="https://developer.arm.com/documentation#f[navigationhierarchiescontenttype]=Performance%20Counters%20Guide">others.</a>
* [Arm GPU Software Developer Errata Notice for Application Developers](https://developer.arm.com/documentation/SDEN-3735689/latest) - An informative document for known driver bugs, application workarounds and fixed driver version.
* [Mali GPU Datasheet](https://developer.arm.com/documentation/102849/0100/?lang=en) - Reference datasheet for device properties such as 'Warp width', 'Max thread count', 'Tile bits/pixel', etc.

## Adreno

* [Snapdragon Profiler.](https://developer.qualcomm.com/software/snapdragon-profiler)
* [Identify application bottlenecks](https://developer.qualcomm.com/sites/default/files/docs/adreno-gpu/snapdragon-game-toolkit/gdg/tutorials/android/identify_application_bottlenecks.html#identify-application-bottlenecks) by using Snapdragon Trace Capture.
* [Available Functionality for Supported Texture Format.](https://developer.qualcomm.com/sites/default/files/docs/adreno-gpu/snapdragon-game-toolkit/gdg/gpu/spec_sheets.html#texture-formats)

## Unreal

* [Maximizing Your Game's Performance in Unreal Engine](https://www.youtube.com/watch?v=GuIav71867E) by Ari Arnbjörnsson - An engaging talk with 4 concrete examples by using built-in tools of UE5. (Few tool configs are desktop-only, but still worth watching.)
* [Profiling and Optimization in UE4](https://www.youtube.com/watch?v=EbXakIuZPFo) by Paulo Souza - An introductory tutorial for identifying performance problems.
* [UE4 Performance and Profiling](https://www.youtube.com/watch?v=hcxetY8g_fs) by Zak Parrish - Comprehensive guidelines for optimization process.
* [UE4 Graphics Profiling](https://www.youtube.com/playlist?list=PLF8ktr3i-U4A7vuQ6TXPr3f-bhmy6xM3S) by Tech Art Aid - A well organized and informative tutorial series for beginners.

## Unity

* [Ultimate guide to profiling Unity games](https://resources.unity.com/games/ultimate-guide-to-profiling-unity-games) - A 70+ page guide on profiling workflow with built-in tools of Unity.
* [Introduction to Profiling in Unity](https://www.youtube.com/watch?v=uXRURWwabF4) by Ciro Continisio - A beginner tutorial on CPU profiler and frame debugger.
* [Tackling Profiling for Mobile Games with Unity and Arm](https://blogs.unity3d.com/2021/03/11/tackling-profiling-for-mobile-games-with-unity-and-arm/) by Mark Harkness - A crisp introduction to mobile game optimization with various tools.
* [Better Together: Integrating Arm Mobile Studio with Unity](https://community.arm.com/developer/tools-software/graphics/b/blog/posts/integrating-arm-mobile-studio-with-unity) by Geraint North - A concrete example of how Streamline annotations make better data interpretation.
