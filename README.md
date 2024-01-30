# jsonnet-docker
This repository offers a Docker image for [google/jsonnet](https://github.com/google/jsonnet.git), providing a streamlined way to utilize Jsonnet within Docker environments. Designed for ease of use and efficiency, our Docker image simplifies the process of integrating Jsonnet into your workflows, ensuring a seamless development experience.

# Usage
To get started, simply pull the latest version of the Docker image using the following command:

```bash
docker pull ghcr.io/mkusaka/jsonnet-docker:latest
```

Running Jsonnet Commands
You can run Jsonnet commands such as jsonnetfmt directly through the Docker container. For example, to format Jsonnet files in your current directory, you can mount your current directory to the container and execute jsonnetfmt:

```bash
docker run --rm -v $(pwd):/workspace -w /workspace ghcr.io/mkusaka/jsonnet-docker:latest jsonnetfmt -i your_file.jsonnet
```

This command mounts your current directory (`$(pwd)`) to `/workspace` inside the container and sets it as the working directory (`-w /workspace`). `jsonnetfmt -i your_file.jsonnet` is then executed to format the specified Jsonnet file in place.

Replace `your_file.jsonnet` with the actual name of your Jsonnet file, or use `*.jsonnet` to apply `jsonnetfmt` to all Jsonnet files in the current directory.

# Tags

Here's a polished introduction for your repository:

This repository offers a Docker image for google/jsonnet, providing a streamlined way to utilize Jsonnet within Docker environments. Designed for ease of use and efficiency, our Docker image simplifies the process of integrating Jsonnet into your workflows, ensuring a seamless development experience.

Usage
To get started, simply pull the latest version of the Docker image using the following command:

bash
Copy code
docker pull ghcr.io/mkusaka/jsonnet-docker:latest
Tags
For a detailed list of all available tags and versions, please visit the package page: https://github.com/mkusaka/jsonnet-docker/pkgs/container/jsonnet-docker

Whether you're working on complex configurations or straightforward projects, this Jsonnet Docker image is crafted to meet your needs, ensuring reliability and consistency across your deployments.
