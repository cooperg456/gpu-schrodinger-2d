# VkTDSE
VkTDSEs (Vulkan Time-Dependent Schrödinger Equation) is a GPU-accelerated solver for the Time-Dependent Schrödinger Equation in 2D, implemented with Vulkan compute shaders. It simulates the evolution of Gaussian wave packets in configurable 2D potential landscapes with real-time visualization.

This project was developed as a final project for PHYS 1321 Computational Methods in Physics (Fall 2025) at the University of Pittsburgh.

<table align="center">
  <tr>
    <td align="center"><img width="240" alt="free_particle" src="https://github.com/user-attachments/assets/9a8a3c74-da5c-451d-8f7d-6f700bc56f58" /></td>
    <td align="center"><img width="240" alt="potential_barrier" src="https://github.com/user-attachments/assets/20b7df68-cd94-4338-9df2-7ff71c62d40f" /></td>
    <td align="center"><img width="240" alt="double_slit" src="https://github.com/user-attachments/assets/140bba7d-e973-467e-a8f1-4ecbbf206959" /></td>
  </tr>
  <tr>
    <td align="center">Free Particle</td>
    <td align="center">Potential Barrier</td>
    <td align="center">Double Slit</td>
  </tr>
</table>


## Dependencies
- [Vulkan SDK](https://vulkan.lunarg.com/)
- [GLFW](https://www.glfw.org/)
- [Vulkan Memory Allocator](https://github.com/GPUOpen-LibrariesAndSDKs/VulkanMemoryAllocator)
- [CMake](https://cmake.org/download/)

## Installation
```zsh
mkdir build && cd build
cmake ..
make -jN
```
where N is the number of system threads.

## Usage
```zsh
./VkTDSE <config>
```
| Config | Description         |
| :----- | :------------------ |
| 0      | Free particle       |
| 1      | Potential barrier   |
| 2      | Double slit barrier |

## Documentation
- [Project Report](docs/PHYS1321_FinalProject.pdf)
- [Presentation Slides](docs/PHYS1321_FinalProject_Slides.pdf)

## License
[MIT](https://choosealicense.com/licenses/mit/)
