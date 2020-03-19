Readme
//////////////////////////////////////////
- Introduction
This project is a raytracer, a program that takes ahigh-level description of a scene (where the objects, lights, and camera are)and produces the image seen through that camera.
//////////////////////////////////////////
- Instruction
To excute this program, you could simply open the "Project_3" file and click on the "Project_3.exe" file.
Follow the instruction pop up, you could enter the ray file you want to check in the following format:
"SampleScenes/rayfilename.ray"
then click on enter, and enter n to check the output image.
The output image would also be updated in the same folder with the name "final_out.png"
Scene(ray) files created are in the "Project_3/Media/SampleScenes" folder named "Scene1.ray" and "Scene2.ray"
The output for these two scenes are in "Project_3" folder.
The animation video is also in "Project_3" folder.
//////////////////////////////////////////
- Code
In project3.cpp line 190 - 226, Currentdir is declared thus we could call the rayTrace (eye,currentDir,recurseDepth) function in the scene.cpp file.
in triangle.cpp line 20 - 54, triangle.testintersection (eye,dir) returns the distance from eye to the intersection point on the triangle object, return 9999999 if no intersection.
in triangle.cpp line 70 - 95, triangle.gettexturecoords() map the texture to triangle.
in sphere.cpp line 12 - 49, sphere.testintersection() returns the distance from eye to the intersection point on the sphere object, return 9999999 if no intersection.
in sphere.cpp line 69 - 98, sphere.gettexturecoords() map the texture to sphere.
in scene.cpp line  16 - 161, raytrace() include ambient light, diffuse light, specular light, reflection, recursive reflection, refraction and recursive refraction.