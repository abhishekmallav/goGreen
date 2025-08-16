# goGreen 🌱

Paint your GitHub contribution graph with backdated commits.

---

## About the Project

**goGreen** is a Python tool that helps you create backdated commits to "paint" your GitHub contribution graph. It automates the process of generating and pushing commits with custom dates, allowing you to visualize patterns or messages on your GitHub profile.

## Features

- Generate any number of backdated commits
- Customizable timezone and random seed for reproducible layouts
- Dry-run mode to preview commit dates
- Automatic push to remote repository
- Beginner-friendly CLI

## Tech Stack / Dependencies

- Python 3.9+
- Standard library: `os`, `json`, `random`, `subprocess`, `argparse`, `datetime`, `zoneinfo`
- Git (must be installed and available in PATH)

## Installation & Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/abhishekmallav/goGreen.git
   cd goGreen
   ```

2. **Ensure Python 3.9+ and Git are installed.**
3. **(Optional) Create a virtual environment:**

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

## Usage

Run the script from your terminal:

```bash
python gogreen.py -n 100 --tz Asia/Kolkata --seed 42
```

**Options:**

- `-n`, `--commits`: Number of commits to generate (default: 100)
- `--tz`, `--timezone`: IANA timezone (default: Asia/Kolkata)
- `--seed`: Random seed for reproducible layout
- `--dry-run`: Print planned dates but don't commit
- `--no-push`: Create commits but don't push at the end

## Configuration

- The script uses `data.json` to store commit data.
- Author and committer info is set in the script (edit as needed).
- Make sure you are inside a Git repository before running.

## Examples

Preview commit dates without making changes:

```bash
python gogreen.py -n 10 --dry-run
```

Generate and push 50 commits in UTC timezone:

```bash
python gogreen.py -n 50 --tz UTC
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Author

Created by [abhishekmallav](https://github.com/abhishekmallav)

## Contribution

Contributions are welcome!

Feel free to fork, open issues or submit pull requests on [GitHub](https://github.com/abhishekmallav/goGreen).

## Contact

For any questions or feedback, please open an issue or reach out via socials below.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abhishekmallav)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:abhimallav1439@gmail.com?subject=Hello%20There&body=Just%20wanted%20to%20say%20hi!)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/abhishekmallav)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=x&logoColor=white)](https://www.x.com/abhishekmallav)

## Credits / Acknowledgments

- Huge credit to the original JavaScript _goGreen_ by [**Harsh Mehta (fenrir2608)**](https://github.com/fenrir2608/goGreen)
