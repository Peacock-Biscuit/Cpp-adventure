# C++ Adventure

## Description

C++ is valuable for data scientists due to its speed and efficiency, which make it ideal for handling large-scale data and complex algorithms. It offers low-level control to optimize performance-intensive tasks. C++ integrates well with other tools like Python and is used in machine learning frameworks like PyTorch. Its versatility allows the creation of custom algorithms and solutions when pre-built options don't suffice. While Python dominates the field, C++ is crucial for tasks requiring top-notch performance.

## Getting Started

In order to solve users' dependency complexity and just test how programs work, a dockerfile is provided to build an image to avoid dependency problems. In case you still do not install docker or docker destop, the following instructions are to install preliminary enviornment in your machines.

### Installation

Docker is available to be downloaded on Homebrew.

```
brew install docker
```

Colima is available on Homebrew, MacPorts, and Nix.

```
# Homebrew
brew install colima

# MacPorts
sudo port install colima

# Nix
nix-env -iA nixpkgs.colima
```

After Colima is installed, there is a step is to build an image based on an existing dockerfile on Colima.

```
colima start

docker build -t cpp-adventure .
```

After an image is built, you could write a command to see a list of your images.

```
docker images
```

To sync with your local directory, a step to run a docker is provided.

```
docker run -it --mount type=bind,src=`pwd`,dst=/app cpp-adventure
```

You could see mounted files under `./Cpp-adventure` show up under `./app` on the docker enviornment.

### How to Run C++ Programs

## Contents

## Reference

[1] C++ primer (5th ed.), Lippman, S. B., Lajoie, J., & Moo, B. E. (2012)

[2] cppreference.com. (n.d.). Cppreference. Retrieved from [cppreference.com](https://en.cppreference.com/w/)

## License
This repository is licensed under the [MIT License](LICENSE) 
