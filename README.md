# Setting Up Jupyter Notebook in VS Code and Opening the Notebook in Google Colab

> **Note:** To view and run this notebook, either set up Jupyter Notebook in VS Code or open the file in Google Colab.

---

## Option 1: Set Up Jupyter Notebook in VS Code

### Prerequisites

* Install Python (3.9 or later recommended)
* Install Visual Studio Code (VS Code)

### Step 1: Install Python

1. Download Python from https://www.python.org/downloads/
2. Run the installer.
3. Make sure to check **"Add Python to PATH"** during installation.
4. Verify the installation:

```bash
python --version
```

or

```bash
python3 --version
```

---

### Step 2: Install VS Code

1. Download VS Code from https://code.visualstudio.com/
2. Install and launch VS Code.

---

### Step 3: Install Required VS Code Extensions

Open VS Code and install the following extensions:

* **Python** (by Microsoft)
* **Jupyter** (by Microsoft)

To install:

1. Open the **Extensions** panel (`Ctrl + Shift + X`).
2. Search for **Python** and install it.
3. Search for **Jupyter** and install it.

---

### Step 4: Create and Activate a Virtual Environment (Recommended)

Open a terminal in VS Code and run:

#### Windows

```bash
python -m venv .venv
.venv\Scripts\activate
```

#### macOS / Linux

```bash
python3 -m venv .venv
source .venv/bin/activate
```

---

### Step 5: Install Jupyter

With the virtual environment activated:

```bash
pip install jupyter ipykernel
```

Verify installation:

```bash
jupyter --version
```

---

### Step 6: Open the Notebook

1. Open the project folder in VS Code.
2. Locate the `.ipynb` notebook file.
3. Double-click the notebook file.
4. VS Code will automatically open the Jupyter Notebook interface.

---

### Step 7: Select the Python Kernel

1. Click **Select Kernel** in the upper-right corner.
2. Choose the Python environment you created.
3. Run cells using:

   * **Run Cell** button
   * `Shift + Enter`

---

## Option 2: Open the Notebook in Google Colab

### Method 1: Upload the Notebook

1. Go to https://colab.research.google.com/
2. Click **Upload**.
3. Select the `.ipynb` notebook file from your computer.
4. The notebook will open automatically.

---

### Method 2: Open from GitHub

If the notebook is stored in a GitHub repository:

1. Go to https://colab.research.google.com/
2. Select the **GitHub** tab.
3. Paste the repository URL or search for the repository.
4. Select the notebook file.

---

### Method 3: Open Directly from Google Drive

1. Upload the notebook to Google Drive.
2. Right-click the notebook file.
3. Select **Open With → Google Colaboratory**.

If Google Colaboratory is not listed:

1. Click **Connect More Apps**.
2. Search for **Colaboratory**.
3. Install and connect it to Google Drive.

---

## Installing Required Python Packages

If the notebook requires additional packages, install them as follows:

### In VS Code

```bash
pip install -r requirements.txt
```

or

```bash
pip install pandas numpy matplotlib scikit-learn
```

### In Google Colab

Run in a notebook cell:

```python
!pip install -r requirements.txt
```

or

```python
!pip install pandas numpy matplotlib scikit-learn
```

---

## Troubleshooting

### Kernel Not Found

Install IPython kernel:

```bash
pip install ipykernel
```

Then restart VS Code.

### ModuleNotFoundError

Install the missing package:

```bash
pip install <package-name>
```

### Google Colab Runtime Issues

Restart the runtime:

**Runtime → Restart Runtime**

---

## You're Ready!

You can now:

* Open and run `.ipynb` notebooks in VS Code.
* Upload and execute notebooks in Google Colab.
* Install additional dependencies as needed.
* Save and share notebooks with others.
