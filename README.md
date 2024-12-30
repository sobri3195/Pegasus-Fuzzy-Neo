# Pegasus Fuzzy-Neo

**Author:** Muhammad Sobri Maulana  

Pegasus Fuzzy-Neo is a Python-based utility designed for fuzz testing, pseudo-random data injection, and data manipulation. It emphasizes safe and ethical data processing techniques. This tool is intended for use in testing applications and systems to ensure robustness and reliability under various scenarios.

## Features

- **Fuzz Testing:** Generate and filter random packets with customizable criteria.
- **Pseudo-Random Data Injection:** Create pseudo-random data for testing scenarios.
- **File Hash Computation:** Compute MD5-like hashes securely using `hashlib`.
- **Key Searching:** Locate specific data within fuzz test results.

## Requirements

- Python 3.7+
- No additional dependencies required (uses standard libraries).

## Installation

Clone the repository and navigate to the project directory:

```bash
$ git clone https://github.com/your-repo/pegasus-fuzzy-neo.git
$ cd pegasus-fuzzy-neo
```

### Function Descriptions

#### `fuzz_packets(filter_func, num_packets=100)`
Generates random packets of varying lengths and filters them based on a user-defined function (`filter_func`).

#### `inject_pseudo_random_data(data_length=32)`
Creates a byte array of pseudo-random data with a specified length (default: 32 bytes).

#### `read_file_and_compute_hash(file_path)`
Reads a file and computes its MD5 hash using Python's `hashlib`. Useful for validating file integrity.

#### `find_key(data, search_value)`
Searches for a specific value in a dataset and returns its index. Returns `-1` if not found.

## Example Scenarios

1. **Fuzz Testing:** Use `fuzz_packets` to generate test data for system robustness testing.
2. **Random Data Injection:** Employ `inject_pseudo_random_data` for simulating edge cases in application behavior.
3. **Hash Verification:** Validate file integrity with `read_file_and_compute_hash`.
4. **Key Search:** Locate specific data in fuzz test results for debugging or analysis.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---
