# Практичне завдання 2 — логістична регресія та федеративне навчання

Виконав: **Новак Сергій, ФЕІ-43с**.

Робота присвячена власній реалізації багатокласової логістичної регресії засобами
NumPy та моделюванню федеративного навчання методом FedAvg на Dry Bean Dataset.

## Структура

- `practice_2_federated_learning.ipynb` — повний звіт, код, графіки та висновки;
- `data/dry_bean_dataset/DryBeanDataset/Dry_Bean_Dataset.xlsx` — набір даних;
- `data/README.md` — джерело та ліцензія даних;
- `requirements.txt` — залежності для локального запуску.

Джерело даних: [UCI Dry Bean Dataset](https://archive.ics.uci.edu/dataset/602/dry+bean),
DOI: 10.24432/C50S4B, ліцензія CC BY 4.0.

## Запуск у VS Code на Windows

1. Відкрийте у VS Code кореневу папку репозиторію.
2. Встановіть розширення **Python** і **Jupyter** від Microsoft.
3. Відкрийте PowerShell-термінал у VS Code та створіть середовище:

   ```powershell
   py -3.11 -m venv .venv
   .\.venv\Scripts\Activate.ps1
   python -m pip install --upgrade pip
   python -m pip install -r requirements.txt
   ```

   Якщо активацію блокує політика PowerShell, лише для поточного термінала виконайте:

   ```powershell
   Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
   .\.venv\Scripts\Activate.ps1
   ```

4. Відкрийте `practice_2_federated_learning.ipynb`.
5. У правому верхньому куті натисніть **Select Kernel** → **Python Environments** →
   `.venv`.
6. Натисніть **Restart Kernel and Run All Cells**.

Ноутбук очікує датасет за шляхом
`data/dry_bean_dataset/DryBeanDataset/Dry_Bean_Dataset.xlsx`, який уже додано у
проєкт. Інтернет для повторного запуску не потрібен.

