# Тестовое задания для Nokia

# Файлы проекта
Название | Описание | Параметры
| --- | --- | --- |
| tests/ | директория с тестовыми файлами | - |
| testNokia.cpp | главный файл с исходным кодом для реализации тестового задания | int argc - количество аргументов, char* argv[] - массив с аругументами |
| testNokia.h |заголовочный файл для главного файла | - | 
| -> printValues.cpp | фукнция для печати таблицы | string* values - указатель на начало матрицы, int countRow - количество строк, int countColumn - количество столбцов, vector<string> vRow - вектор с именами строк, vector<string> vColumn - вектор с именами столбцов |
| -> printValues.h | заголовочный файл с прототипом функции | - |
| -> calc.cpp | функция для вычисления значений в таблице, возвращает true/false - успешно или нет | string* values - указатель на начало матрицы, int countRow - количество строк, int countColumn - количество столбцов, vector<string> vRow - вектор с именами строк, vector<string> vColumn - вектор с именами столбцов |
| -> calc.h | заголовочный файл с прототипом функции | - |
| --> calculateCell.cpp | функция для вычисления значений в ячейке, возвращает true/false - успешно или нет | string cell - строка с одержимым ячейки, int countColumn - количество столбцов, vector<string> vRow - вектор с именами строк, string* values - указатель на начало матрицы, int countRow - количество строк, int i - позиция в строке текущей ячейки, int j - позиция в столбце текущей ячейки |
| --> calculateCell.h | заголовочный файл с прототипом функции | - |
| ---> getValue.cpp | функция для получения значения ячейки | vector<string> vRow - вектор с именами строк, vector<string> vColumn - вектор с именами столбцов, string operand - строка с именем ячейки, string* values - указатель на начало матрицы, int countRow - количество строк, int& i - позиция в строке текущей ячейки, int& j - позиция в столбце текущей ячейки |
| ---> getValue.h | заголовочный файл с прототипом функции | - |
| Makefile_unix | make-файл для сборки и тестирования программы под unix | без параметров - сборка исполняемого файло (testNokia.exe), test - выполнение тестов, clean - удаление exe-файла |
| Makefile_windows | make-файл для сборки и тестирования программы под windows | без параметров - сборка исполняемого файло (testNokia.exe), test - выполнение тестов, clean - удаление exe-файла |

# Руководство
### Пример выполнения:
1. Вызов `make` (сборка testNokia.exe).
2. Вызов `make test` (выполнение тестов).
