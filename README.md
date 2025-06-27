# LyfSim

LyfSim is a life simulator that models a person's life from age 18 to death, incorporating education, career, health, and random life events based on statistical rules. It supports both a command-line interface (CLI) and a graphical user interface (GUI) built with Python's `tkinter`.

![GUI Screenshot](https://github.com/user-attachments/assets/31861396-e69b-45af-80b7-a72222eef6e2)

## Features

* **Simulate a Life**: Generate a unique life story with realistic demographics, education paths, careers, and income based on simplified real-world data.
* **GUI Mode**:

  * View life summaries in a scrollable window.
  * Set batch size (1–100) to simulate multiple lives at once.
  * Save session history to a text file.
  * Re-run simulations with a "Run Again" button.
* **CLI Mode**: Run in the terminal with plain-text output.
* **Cross-Platform**: Works on Windows, macOS, and Linux.
* **Data-Driven**: Uses simplified income data based on BLS estimates (auto-generated on first run).

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Innomen/LyfSim.git
cd LyfSim
```

### 2. Ensure Python 3 Is Installed

LyfSim requires **Python 3.6+** with `tkinter`.

On Linux, you may need to install `tkinter` separately:

```bash
# Example for Arch-based systems
sudo pacman -S tk
```

## Running the Simulator

### GUI Mode (Default)

```bash
python3 lyfsim.py
```

### CLI Mode

```bash
python3 lyfsim.py --cli
```

## Usage

### GUI Mode

* Launch with `python3 lyfsim.py`
* Use the "Batch Size" spinner to select how many lives to simulate (1–100).
* Click **"Run Again"** to simulate a new batch.
* Click **"Save Session"** to export all simulated lives to a `.txt` file.

### CLI Mode

* Run `python3 lyfsim.py --cli` for a single life simulation in the terminal.

## Files

* `lyfsim.py` — Core simulation logic with GUI/CLI interface.
* `data/occupation_income.csv` — Auto-generated on first run with simplified income data.

## Development

* **Contributing**: Pull requests are welcome! Open an issue first to discuss changes.
* **Dependencies**: Pure Python, no external libraries beyond the standard library.
* **Packaging**: To create a standalone executable:

```bash
# Example with zipapp
python3 -m zipapp lyfsim.py
# Or consider using PyInstaller for more advanced packaging
```

## License

MIT License — see `LICENSE` file for details.

## Acknowledgments

* Inspired by statistical life simulation concepts.
* Income data structure loosely based on simplified Bureau of Labor Statistics estimates.

---

**Last updated:** June 27, 2025
