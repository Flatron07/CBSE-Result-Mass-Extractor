# CBSE-Result-Mass-Extractor
This repo will help to extract cbse results in mass in given roll numbers.

# Selenium Result Automation Tool

A Python-based browser automation project built using Selenium WebDriver. The project demonstrates automated form interaction, checkpoint-based progress tracking, session recovery, and data collection through a Chromium-based browser.

## Overview

This project automates repetitive web form submissions by:

- Launching a Chromium-based browser
- Filling form fields automatically
- Submitting requests
- Monitoring responses
- Saving successful responses
- Supporting resume functionality through checkpoints
- Maintaining progress statistics

The project is intended as a demonstration of browser automation, Selenium workflows, and long-running task management.

---

## Features

### Browser Automation
- Automated form filling
- Keyboard interaction support
- Dynamic page navigation
- Automatic page reload handling

### Progress Tracking
- Checkpoint system
- Resume after interruption
- Persistent progress storage
- Automatic recovery from previous sessions

### Data Collection
- Response detection
- Screenshot capture
- Organized output storage
- Result indexing

### Session Management
- Browser initialization
- Custom Chromium configuration
- Graceful shutdown handling
- Resource cleanup

### Logging
- Real-time progress updates
- Attempt tracking
- Runtime statistics
- Completion summaries

---

## Tech Stack

- Python
- Selenium WebDriver
- ChromeDriver
- Chromium-Based Browser (Chrome/Brave)

---

## Project Structure

```text
project/
│
├── main.py
├── checkpoint.txt
├── results/
│   ├── result_1.png
│   ├── result_2.png
│   └── ...
│
└── README.md
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/selenium-result-automation.git
cd selenium-result-automation
```

### Install Dependencies

```bash
pip install selenium
```

### Download ChromeDriver

Download the version matching your browser from:

https://developer.chrome.com/docs/chromedriver/

Update the path in the script:

```python
CHROMEDRIVER_PATH = r"C:\chromedriver\chromedriver.exe"
```

---

## Configuration

Configure the following parameters before running:

```python
RESULT_URL = "YOUR_TARGET_URL"
START_ID   = ...
END_ID     = ...
OUTPUT_DIR = "results"
```

Update browser executable path if required:

```python
BRAVE_PATH = r"C:\Program Files\BraveSoftware\Brave-Browser\Application\brave.exe"
```

---

## How It Works

1. Launches a Chromium-based browser.
2. Opens the configured target page.
3. Fills required form fields.
4. Submits the form.
5. Checks whether a valid response is returned.
6. Saves successful responses as screenshots.
7. Stores progress in a checkpoint file.
8. Resumes automatically after interruption.
9. Generates runtime statistics.

---

## Key Components

### Checkpoint System

Functions:

```python
save_checkpoint()
load_checkpoint()
delete_checkpoint()
```

Purpose:
- Resume interrupted runs
- Prevent loss of progress
- Reduce repeated work

### Browser Management

Functions:

```python
reload()
clear_and_type()
```

Purpose:
- Handle page refreshes
- Simulate user interaction
- Maintain browser stability

### Result Processing

Features:

- Response detection
- Screenshot storage
- Sequential indexing
- Output organization

---

## Output

Successful responses are stored inside:

```text
results/
```

Example:

```text
results/
├── result_1.png
├── result_2.png
├── result_3.png
```

---

## Learning Objectives

This project demonstrates:

- Selenium WebDriver automation
- Browser interaction
- Form automation
- Progress persistence
- Checkpoint-based recovery
- File management
- Long-running task handling
- Exception handling

---

## Future Improvements

- Multi-threaded execution
- Headless browser support
- CSV export
- Database integration
- Docker support
- Advanced logging
- GUI dashboard
- Cloud execution support

---

## Author

Bhaskar Negi

## License

This project is intended for educational and research purposes.
