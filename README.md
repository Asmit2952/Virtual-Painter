# Virtual-Painter

This is a simple C++ project made with OpenCV library which is used to detect an object color manually and then draw with that color in real-time on the output screen.

First install OpenCV for Windows by [following these steps](https://dev.to/asmit2952/installing-opencv-on-windows-for-c-326i)

The project has two .cpp files (color_picker and virtual_painter).
The code which I have written is manual operated, which means you have to add colors manually to `virtual_painter.cpp` with the help of `color_picker.cpp`

To do that, follow these steps:
1. Exclude `virtual_painter.cpp` from the Project file.
2. Include `color_picker.cpp`.
3. Run `color_picker.cpp`. You will see three windows named `Images`, `Images Mask` and `Trackbars`
4. Take a marker of any color, and move the sliders in `Trackbar` window in such a way that only that specific color of the object should be visible on `Image Mask` window.

![color_picker.cpp](https://github.com/Asmit2952/Virtual-Painter/blob/master/Images/Screenshot%20(63).png)

5. Keep in mind that there shouldn't be any noise in `Image Mask` window.
6. Now copy the latest values from the `Output Screen`.

![output_screen](https://github.com/Asmit2952/Virtual-Painter/blob/master/Images/Screenshot%20(64).png)

7. Exclude `color_picker.cpp` and include `virtual_painter.cpp`.
8. Paste those copied values in `vector<vector<int>> myColors`.

![myColor](https://github.com/Asmit2952/Virtual-Painter/blob/master/Images/Screenshot%20(65).png)

9. Next, find the BGR value of your object color and paste it in `vector<Scalar> myColorValues`

![myColorValues](https://github.com/Asmit2952/Virtual-Painter/blob/master/Images/Screenshot%20(66).png)

10. Execute the code, and new color should be displayed when it detects the object of that color

If you have any issues, feel free to contact me😉
