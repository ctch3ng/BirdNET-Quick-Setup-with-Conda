# BirdNET Quick Setup with Conda

This repository provides a quick setup guide for creating a virtual environment using Conda and installing [BirdNET Analyzer](https://github.com/kahst/BirdNET-Analyzer).

## Prerequisites
Ensure you have the following installed on your system:
- [Conda](https://docs.conda.io/en/latest/miniconda.html) (Miniconda or Anaconda)

## Setup Instructions

### Step 1: Create and Activate a Conda Environment
Run the following commands to create and activate a Conda environment with Python 3.10:
```bash
conda create -n py310_TF python=3.10 -y
conda activate py310_TF
```

### Step 2: Install Dependencies
Install `ffmpeg` and `git` from Conda:
```bash
conda install conda-forge::ffmpeg
conda install git
```

### Step 3: Clone BirdNET Analyzer Repository
Clone the BirdNET Analyzer repository to your local machine:
```bash
git clone https://github.com/kahst/BirdNET-Analyzer.git
```

Go inside the directory (i.e. folder) `BirdNET-Analyzer`
```bash
cd BirdNET-Analyzer
```

### Step 4: Install Python Dependencies
Install the required Python packages using `pip`:
```bash
pip install -r requirements.txt
```

## Running BirdNET Analyzer

### Command-Line Analysis
Run the analyzer using the following command:
```bash
python -m birdnet_analyzer.analyze
```

### Graphical User Interface (GUI)
Launch the GUI with the command:
```bash
python -m birdnet_analyzer.gui
```

## Notes
- Ensure your `conda` environment is activated before running any BirdNET commands.
- Refer to the [official BirdNET Analyzer documentation](https://github.com/kahst/BirdNET-Analyzer) for advanced usage and configuration.

## License
This repository follows the license of the original [BirdNET Analyzer](https://github.com/kahst/BirdNET-Analyzer). Please check the original repository for detailed license information.

## Contribution
Feel free to submit issues or pull requests for improvements or suggestions.
