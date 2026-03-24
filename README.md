# Resume - Federico Gualdi

This repository contains the LaTeX source code for my resume/CV as a software engineer, with a focus on distributed systems, backend development and cloud-native architectures.

## View the Resume
For full details, you can view the PDF: [Federico Gualdi - Resume.pdf](./Federico%20Gualdi%20-%20Resume.pdf)

## Structure
- Modular LaTeX files for easy editing and maintenance
- Custom class and fonts for a modern, clean look
- Sections: Profile, Skills, Work Experience, Projects, Entrepreneurship, Education


## Build the Resume

### Requirements

Install the required LaTeX packages:

```bash
    make install
```

### Build using Make

To generate the PDF, run:

```bash
    make export
```

This will:

- compile the LaTeX file with XeLaTeX
- place temporary files in the build/ directory
- export the final PDF to the parent folder

### Custom output filename

You can choose a custom PDF name:

```bash
make export FILENAME="Mario Rossi Resume"
```

### Clean build files

To remove temporary files:

```bash
make clean
```

### Notes

- The FILENAME variable controls the name of the output PDF
- File names with spaces are supported but must be quoted
- The build directory is used to keep auxiliary files separate from the project root