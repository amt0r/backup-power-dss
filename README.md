# backup-power-dss

Decision Support System (DSS) to help users choose the optimal backup power solution based on their specific needs, such as budget, required capacity, fuel type, and mobility. 

This expert system utilizes a questionnaire-based approach. The answers provided by the user are processed by an Inference Engine that calculates a score for each available alternative power source (e.g., generators, portable power stations, solar panels) and provides recommendations.

## Features

- **Interactive Questionnaire:** Assesses user requirements (budget, noise level, location, needed power, etc.).
- **Inference Engine:** Evaluates answers against predefined rules and scoring logic.
- **Top Recommendations:** Outputs sorted options with percentage matches and detailed explanations (pros and cons).
- **Admin Panel:** Allows authentication and dynamic management of questions, options, and scoring rules without modifying the code.
- **Import / Export:** Easily migrate database rules and state via JSON files.
- **PyQt6 GUI:** Clean and modern graphical user interface.
- **SQLite Database:** Lightweight and fast local storage for state and inference rules.

## Requirements

- Python 3.9+
- `PyQt6`

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/backup-power-dss.git
   cd backup-power-dss
   ```

2. (Optional) Create a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows use: .venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install PyQt6
   ```

## Usage

To launch the application, run:
```bash
python main.py
```
*Note: The application will automatically initialize the database `dss_energy.db` and populate it with initial data if it doesn't exist.*

### Running Tests
To run the built-in test suite:
```bash
python -m unittest tests.py
```

## Admin Access
- **Username:** `admin`
- **Password:** `admin123`

## Topics
`decision-support-system`, `expert-system`, `python`, `pyqt6`, `backup-power`, `sqlite`
