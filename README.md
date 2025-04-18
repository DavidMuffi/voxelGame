Vulkan Voxel Game (C)
A Minecraft-like game engine using Vulkan in C, aiming to provide ultra-optimized performance, full control over the hardware, and a modular foundation for future expansion.

🚀 Installation
Prerequisites
To run this project, you will need to install the following tools and libraries:

Vulkan SDK
Download and install the Vulkan SDK from LunarG Vulkan SDK. Make sure to follow the installation instructions for your platform.

GLFW
GLFW is a library that makes creating windows and handling input events easier. To install it:

Linux:
sudo apt-get install libglfw3 libglfw3-dev

CMake (Optional but recommended for larger projects)

Linux:
sudo apt-get install cmake

GPU Drivers
Ensure that you have the latest drivers for your GPU that support Vulkan.

🛠 Build the Project
Set Up Environment Variables
In your terminal or command prompt, make sure the Vulkan SDK is set up correctly:

Linux / MacOS: Add the following lines to your .bashrc or .zshrc file:
export VULKAN_SDK=/path/to/vulkan-sdk
export PATH=$VULKAN_SDK/bin:$PATH
export LD_LIBRARY_PATH=$VULKAN_SDK/lib:$LD_LIBRARY_PATH
export VK_ICD_FILENAMES=$VULKAN_SDK/etc/vulkan/icd.d/nvidia_icd.json
export VK_LAYER_PATH=$VULKAN_SDK/etc/vulkan/explicit_layer.d

Then, reload the terminal with:
source ~/.bashrc   # o ~/.zshrc

Build the Project
cd voxelGame
mkdir build
cd build

Run CMake to configure the project:
cmake ..
make

📖 Usage
Once the project is built, run the generated binary to see the Vulkan window in action.

📝 Features
Basic block engine using Vulkan for rendering.

Procedural sine-wave shaders for dynamic block texturing.

Full control over the graphics pipeline and GPU memory.

Shader and buffer management system for handling multiple block types.

🛠 Next Steps
Add procedural terrain generation (such as Perlin Noise to create worlds).

Implement chunk management for efficient loading/unloading of blocks.

Add interaction support (player movement, collisions, etc.).

🔗 Resources
Vulkan API Doc
https://docs.vulkan.org/spec/latest/index.html
GLFW Doc
https://www.glfw.org/documentation
