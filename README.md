# Windows UAC Integrity & Environment Security Research

> Windows UAC Bypass in Python & CPP

## About

Ce projet est un outil de recherche en cybersécurité développé pour illustrer et analyser la technique de contournement de l'UAC (User Account Control) dite du "Mock SystemRoot".
Il démontre comment un processus avec un niveau d'intégrité moyen peut interagir avec les interfaces COM du Planificateur de tâches pour manipuler l'environnement utilisateur.

## Features

* **Vérification automatique** de l'état des services Windows.
* **Manipulation du registre** pour isoler les variables d'environnement.
* **Pilotage d'interfaces COM** du Task Scheduler pour l'exécution.
* **Architecture modulaire** avec composant Payload en C++.

## Quick Start

### Prerequisites

```bash
Python += v3.12
pywin32
ctypes
```

### Installation

1. Clone the repository

```bash
git clone https://github.com/936erpl/uac.git
cd uac
```

2. Install dependencies

```bash
Option 1 :
pip install -r requirements.txt

or (both are the same)

Option 2 :
pip install pywin32
pip install ctypes
```

3. Start the project

```bash
python bypass.py
```

## Documentation

For more details, see the complete documentation:

```text
./uac/docs/UAC-Documentation.md
```

## Technology Stack

* **Automation Script:** Python 3 (Modules : `ctypes`, `winreg`)
* **Windows API Bindings:** `pywin32` (`win32com`, `pythoncom`)
* **Payload Component:** C++17, Win32 Native API

## Usage Example

```bash
// Basic example of the bypass.py (opens a admin cmd without triggering uac)
C:\Users\redacted\Desktop\redacted\redacted>python bypass.py

                    .___       ___.             ________________  ________
  _____ _____     __│ _╱____   ╲_ │__ ___.__.  ╱  _____╱╲_____  ╲╱   __   ╲
 ╱     ╲╲__  ╲   ╱ __ │╱ __ ╲   │ __ <   │  │ ╱   __  ╲   _(__  <╲____    ╱
│  Y Y  ╲╱ __ ╲_╱ ╱_╱ ╲  ___╱   │ ╲_╲ ╲___  │ ╲  │__╲  ╲ ╱       ╲  ╱    ╱
│__│_│  (____  ╱╲____ │╲___  >  │___  ╱ ____│  ╲_____  ╱╱______  ╱ ╱____╱
      ╲╱     ╲╱      ╲╱    ╲╱       ╲╱╲╱             ╲╱        ╲╱

>>> [!] Successful.
```

## Contributing

Contributions are welcome to help improve the stability of the audit scripts or to document new Windows security mitigations. To contribute:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/NewFeature`).
3. Commit your changes (`git commit -m "Add some New Features"`).
4. Push to the branch (`git push origin feature/NewFeature`).
5. Open a Pull Request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more information.

## Author

**639**

* GitHub: https://github.com/936erpl
* Contact: cybermuxcorp@gmail.com
* Discord: `reversinglabs`

## Support

If you find this project useful, consider giving it a star on GitHub.

---

<div align="center">
  Built and maintained by <strong>639</strong>
</div>
