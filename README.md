# 2048
<!-- ![Build](https://github.com/INFOM126-Automated-Software-Engineering/2048-groupe-erasmus/actions/workflows/ci.yml/badge.svg) -->
![Java](https://img.shields.io/badge/Java-11%2B-blue)
![License](https://img.shields.io/github/license/INFOM126-Automated-Software-Engineering/2048-groupe-erasmus)

This project is an implementation of the classic **2048** game.
This **Java** implementation of this game uses **Maven** for build and dependency management automation.

## Requirements
- Java JDK **11 or higher**
- Maven **3.6.0 or higher**

## Features
- Classic 2048 gameplay
- Modular Java architecture
- Maven-based build

## Getting Started
To run this project, you first need to download the code for the project. For this clone, this repository with the command:
```bash
git clone https://github.com/INFOM126-Automated-Software-Engineering/2048-groupe-erasmus.git
```

Then, you need to build the project with the command:
```bash
mvn clean install
```

Now, you can run the game with:
```bash
mvn exec:java '-Dexec.mainClass=be.unamur.game2048.Game'
```

## Contributing
If you want to contribute to the project, please feel free to read our [contributor guide](CONTRIBUTING.md).

Please read our [Code of Conduct](CODE_OF_CONDUCT.md) before contributing.

## Reporting Issues
### Security vulnerabilities
If you discover a security vulnerability, **please do not open a public issue**.
Instead, follow the process described in [SECURITY.md](SECURITY.md) to report security issues responsibly.

### Reporting Bugs
For non-security related bugs, please open a GitHub issue and use the **Bug Report** [template](.github/ISSUE_TEMPLATE/bug_report.md).

## Contact
To contact us for any questions / issues, please contact us on GitHub 
[issues](https://github.com/INFOM126-Automated-Software-Engineering/2048-groupe-erasmus/issues) / 
[pull requests](https://github.com/INFOM126-Automated-Software-Engineering/2048-groupe-erasmus/pulls) / 
[discutions](https://github.com/INFOM126-Automated-Software-Engineering/2048-groupe-erasmus/discussions).

## License
This project is open source and licensed under the GNU Free Documentation License. See the [license](LICENSE) for more details.
