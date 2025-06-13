# Setup

To use C++ on *Microsoft Visual C++*, change/enable these properties in *Project > Properties > Configuration Properties > C/C++ > Language*:

- C++ Language Standard -> ```Preview - Features from the Latest C++ Working Draft (/std:c++latest)``` .
- Enable Experimental C++ Standard Library Modules -> ```Yes (/experimental:module)```.
- Build ISO C++ 23 Standard Library Modules -> ```Yes```.

Then, go to *Tools > Get tools and features*. The Visual Studio Installer window should open. In *Individual Components*, search for "Modules", and install the component: ```C++ Modules for v143 build tools (x64/x86 - experimental)```.


#### Test if the following code works properly:
```cpp
import std;

int main()
{
    std::print("Hello, World!");
}
```
```
Hello, World!
```

If you have any trouble while testing, try changing the Project to other Configuration and Platform (Example: *Release* and *x86*).