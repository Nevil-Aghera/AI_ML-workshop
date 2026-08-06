# 🐼 Pandas — Practice & Concepts Notebook

A hands-on **Pandas fundamentals notebook** covering Series, flexible CSV reading, missing-value handling, `replace()`, `interpolate()`, and `.loc`/`.iloc` indexing.

---

## 📁 Project Files

| File | Description |
|---|---|
| 📓 `Pandas_AI_Ml.ipynb` | Main Jupyter Notebook — Pandas concepts, examples & practice |
| 📊 `Data/Fortune_10.csv` | ⚠️ Referenced dataset (**not included**) |
| 📊 `Data/Fortune_10 - Copy.csv` | ⚠️ Referenced dataset with NaN values (**not included**) |
| 📊 `Data/Fortune_5 nan values.csv` | ⚠️ Referenced dataset for missing-value demos (**not included**) |
| 📊 `Data/student_results - copy.csv` | ⚠️ Referenced dataset for interpolation demo (**not included**) |
| 📊 `Data/student_results.xls` | ⚠️ Referenced dataset for `.loc`/`.iloc` demo (**not included**) |

> ⚠️ **Note:** All 5 data files are referenced via relative `Data\...` / `Data//...` paths but weren't part of this upload. Place them in a `Data/` folder next to the notebook before running.

---

## 🔍 What's Inside the Notebook

The notebook has **74 cells** covering the following topics:

### 🧵 1. Pandas Series
- 🔢 Scalar & list-based Series creation
- 🏷️ Custom index, dtype, and name
- 🎯 Indexing & filtering (`sr_index[3]`, `sr_index[sr_index < 2]`)
- ➕ Series arithmetic (element-wise addition)

### 📥 2. Reading CSV Files — Flexible Options
- 📄 Basic `read_csv()`
- 🔢 `nrows` — limit rows read
- 📊 `usecols` — select specific columns
- ⏭️ `skiprows` — skip specific rows
- 🆔 `index_col` — set custom index (by name or position)
- 📋 `header` — custom header row
- 🏷️ `names` — rename columns on load
- 🔤 `dtype` — force column data types

### 🕳️ 3. Handling NaN / Missing Values
- 🔍 Custom `na_values` (string & column-specific)
- ⚙️ `keep_default_na`, `na_filter`
- ❓ `.isnull()`, `.notnull()` (with `.sum()`)
- 🧹 `.dropna()` — by axis, `how`, `thresh`, `subset`
- 🩹 `.fillna()` — dict-based fill values
- ⏩ `.ffill()` / ⏪ `.bfill()` (with `limit`)

### 🔄 4. Replace Values
- 🔁 `.replace()` — single value, numeric value, regex-based replacement
- ✏️ Column-specific replacement (`df["Industry"].replace(...)`)

### 📈 5. Interpolation
- 🧮 `.interpolate()` — fill numeric gaps only (chars untouched)
- 📐 Linear interpolation method

### 🎯 6. `.loc` and `.iloc` Indexing
- 🏷️ `.loc[]` — label-based selection (rows, row lists, cell, conditional filtering, column selection)
- 🔢 `.iloc[]` — integer-position-based selection (rows, row lists, columns)

---

## 🛠️ Tech Stack

- 🐍 Python
- 🐼 Pandas
- 🔢 NumPy

---

## ▶️ How to Run

1. 📥 Clone/download this project folder
2. 📦 Install dependencies:
   ```bash
   pip install pandas numpy
   ```
3. 📁 Create a `Data/` folder with the 5 referenced CSV/XLS files
4. 📓 Open `Pandas_AI_Ml.ipynb` in Jupyter Notebook / JupyterLab / VS Code
5. ▶️ Run all cells in order

---

## ✅ Status

- ✔️ Series basics covered
- ✔️ Flexible CSV reading options covered
- ✔️ Missing-value detection & handling covered
- ✔️ Replace & interpolate operations covered
- ✔️ `.loc` / `.iloc` indexing covered
- ⚠️ Referenced data files not included — must be supplied separately
- ⚠️ Minor typos in code (`na_filter='False'` as string, `mrthod` instead of `method`) — may cause unexpected behavior or errors when run
