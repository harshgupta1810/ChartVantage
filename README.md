# ChartVantage

ChartVantage is a Python-based project designed to identify and analyze chart patterns in financial time series data. This tool enables traders and analysts to recognize key patterns in stock price movements, aiding in market predictions and decision-making.

---

## Features

- **Pattern Recognition**: Detects over 20 classic technical patterns, including:
  - Bullish Flag, Bearish Flag
  - Head and Shoulders, Inverse Head and Shoulders
  - Ascending Triangle, Descending Triangle
  - Cup with Handle, Rounding Bottom, and more.
- **Data Retrieval**: Fetches historical stock data using Yahoo Finance API.
- **Customizable Analysis**: Define the maximum number of bars for patterns to develop.
- **Pattern Ranking**: Provides a priority ranking for identified patterns based on significance.

---

<p align="center">
    <img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" align="center" width="30%">
</p>
<p align="center"><h1 align="center"><code>❯ REPLACE-ME</code></h1></p>
<p align="center">
	<em><code>❯ REPLACE-ME</code></em>
</p>
<p align="center">
	<!-- local repository, no metadata badges. --></p>
<p align="center">Built with the tools and technologies:</p>
<p align="center">
	<img src="https://img.shields.io/badge/Python-3776AB.svg?style=default&logo=Python&logoColor=white" alt="Python">
</p>
<br>

##  Table of Contents

- [ Overview](#-overview)
- [ Features](#-features)
- [ Project Structure](#-project-structure)
  - [ Project Index](#-project-index)
- [ Getting Started](#-getting-started)
  - [ Prerequisites](#-prerequisites)
  - [ Installation](#-installation)
  - [ Usage](#-usage)
  - [ Testing](#-testing)
- [ Project Roadmap](#-project-roadmap)
- [ Contributing](#-contributing)
- [ License](#-license)
- [ Acknowledgments](#-acknowledgments)

---

---

---

##  Project Structure

```sh
└── /
    ├── candlestick_chart
    │   ├── backend.ipynb
    │   └── candlestick_chart.py
    ├── candlestick_pattern
    │   ├── candle_names.py
    │   ├── candle_rankings.py
    │   ├── candlestick_pattern.py
    │   └── find_candlestick_pattern.ipynb
    └── chart_pattern
        ├── backend.ipynb
        ├── find_extrema.py
        ├── pattern_list.py
        ├── reconise_pattern.py
        ├── target_stoploss.py
        └── type_pattern.py
```


###  Project Index
<details open>
	<summary><b><code>/</code></b></summary>
	<details> <!-- __root__ Submodule -->
		<summary><b>__root__</b></summary>
		<blockquote>
			<table>
			</table>
		</blockquote>
	</details>
	<details> <!-- candlestick_chart Submodule -->
		<summary><b>candlestick_chart</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='/candlestick_chart/backend.ipynb'>backend.ipynb</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='/candlestick_chart/candlestick_chart.py'>candlestick_chart.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			</table>
		</blockquote>
	</details>
	<details> <!-- candlestick_pattern Submodule -->
		<summary><b>candlestick_pattern</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='/candlestick_pattern/candlestick_pattern.py'>candlestick_pattern.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='/candlestick_pattern/candle_names.py'>candle_names.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='/candlestick_pattern/candle_rankings.py'>candle_rankings.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='/candlestick_pattern/find_candlestick_pattern.ipynb'>find_candlestick_pattern.ipynb</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			</table>
		</blockquote>
	</details>
	<details> <!-- chart_pattern Submodule -->
		<summary><b>chart_pattern</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='/chart_pattern/backend.ipynb'>backend.ipynb</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='/chart_pattern/find_extrema.py'>find_extrema.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='/chart_pattern/pattern_list.py'>pattern_list.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='/chart_pattern/reconise_pattern.py'>reconise_pattern.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='/chart_pattern/target_stoploss.py'>target_stoploss.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='/chart_pattern/type_pattern.py'>type_pattern.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			</table>
		</blockquote>
	</details>
</details>

---
##  Getting Started

###  Prerequisites

Before getting started with , ensure your runtime environment meets the following requirements:

- **Programming Language:** Python


###  Installation

Install  using one of the following methods:

**Build from source:**

1. Clone the  repository:
```sh
❯ git clone https://github.com/harshgupta1810/ChartVantage.git



---



<details closed>
<summary>Contributing Guidelines</summary>

1. **Fork the Repository**: Start by forking the project repository to your LOCAL account.
2. **Clone Locally**: Clone the forked repository to your local machine using a git client.
   ```sh
   git clone https://github.com/harshgupta1810/ChartVantage.git
   ```
3. **Create a New Branch**: Always work on a new branch, giving it a descriptive name.
   ```sh
   git checkout -b new-feature-x
   ```
4. **Make Your Changes**: Develop and test your changes locally.
5. **Commit Your Changes**: Commit with a clear message describing your updates.
   ```sh
   git commit -m 'Implemented new feature x.'
   ```
6. **Push to LOCAL**: Push the changes to your forked repository.
   ```sh
   git push origin new-feature-x
   ```
7. **Submit a Pull Request**: Create a PR against the original project repository. Clearly describe the changes and their motivations.
8. **Review**: Once your PR is reviewed and approved, it will be merged into the main branch. Congratulations on your contribution!
</details>

<details closed>
<summary>Contributor Graph</summary>
<br>
<p align="left">
   <a href="https://LOCAL{///}graphs/contributors">
      <img src="https://contrib.rocks/image?repo=/">
   </a>
</p>
</details>

---

##  License

This project is protected under the [SELECT-A-LICENSE](https://choosealicense.com/licenses) License. For more details, refer to the [LICENSE](https://choosealicense.com/licenses/) file.

---

##  Acknowledgments

- List any resources, contributors, inspiration, etc. here.

---
