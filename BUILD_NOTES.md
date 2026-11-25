# Build and publication notes

This is a cleaned copy of the original CS-330 Windows Visual Studio project, not a standalone build. Source and texture files are unchanged. Original instructor attribution is preserved.

## Local build layout

The original project expects the course-provided CS330Content directory two levels above the project folder. For example:

```
CS330Content/
  3DShapes/
  Utilities/
  Libraries/
  Projects/
    Final Project/
      7-1_FinalProjectMilestones.sln
      7-1_FinalProjectMilestones.vcxproj
      Source/
      Textures/
```

The earlier CS-330 Final Project.zip contains CS330Content support files. Use that archive locally to reconstruct the layout; do not publish it without checking permissions. The project references ShapeMeshes.cpp, ShaderManager.cpp, stb_image.h, camera.h, vertexShader.glsl and fragmentShader.glsl, plus GLFW, GLEW and GLM. It links glew32.lib, glfw3.lib and opengl32.lib (also glu32.lib in Release). The project uses Visual Studio 2022 (v143), Windows SDK 10 and Win32 Debug/Release configurations. A matching GLEW runtime DLL may need to be available beside the executable or on PATH. Run with the project folder as working directory for relative texture and shader paths. The project also lists two external image references under Utilities/textures; these are retained unchanged.

## Before publishing

Confirm SNHU permits public redistribution of the starter framework and modified coursework. Confirm rights to each texture image, including any logos or third-party content. Retain instructor attribution and any applicable licenses. This archive includes the original source and textures for private review; inclusion is not a license clearance. External libraries and compiled binaries are not bundled. Do not replace your existing GitHub README or screenshot with this archive. Once permissions are confirmed, upload the approved files individually, preserving directory structure. If permission is unclear, keep the source private and showcase the screenshot and project description instead.

## Verification

Archive contents were checked; no compilation or runtime testing was performed. Original project paths were deliberately preserved rather than claiming a portable build.
