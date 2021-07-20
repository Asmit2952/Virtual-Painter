# Virtual-Painter

First install OpenCV for Windows by [following these steps](https://dev.to/asmit2952/installing-opencv-on-windows-for-c-326i)

The project has two .cpp files (color_picker and virtual_painter).
The code which I have written is manual operated, which means u have to add colors manually to `virtual_painter.cpp` with the help of `color_picker.cpp`

To do that, follow these steps:
1. Exclude `virtual_painter.cpp` from the Project file.
2. Include `color_picker.cpp`.
3. Run `color_picker.cpp`. You will see three windows named `Images`, `Images Mask` and `Trackbars`
4. Take a marker of any color, and move the sliders in `Trackbar` window in such a way that only that specific color of the object should be visible on `Image Mask` window.
5. Keep in mind that there shouldn't be any noise in `Image Mask` window.
6. Now copy the latest values from the `Output Screen`.
7. Exclude `color_picker.cpp` and include `virtual_painter.cpp`.
8. Paste those copied values in `vector<vector<int>> myColors`.
9. Next, find the BGR value of your object color and paste it in `vector<Scalar> myColorValues`
10. Execute the code, and new color should be displayed when it detects the object of that color
