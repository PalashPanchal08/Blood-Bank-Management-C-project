# Blood Bank Management — IU2541230057 / CPP37

Console-based C++ OOP project prepared from the supplied project blueprint.

## Requirements
- C++11 or newer compiler (g++, MinGW-w64, or an IDE such as Code::Blocks / Visual Studio).
- Run the program from the project root so the `Data/` directory is used.

## Compile
**Windows (MinGW):**
```bat
g++ -std=c++11 -Wall -Wextra -pedantic main.cpp -o BloodBank.exe
BloodBank.exe
```
**Linux/macOS:**
```bash
g++ -std=c++11 -Wall -Wextra -pedantic main.cpp -o BloodBank
./BloodBank
```
A `compile.bat` file is included for Windows.

## Features
- Add, display, search, update, and delete donor/patient/blood-unit/request records where applicable.
- Blood collection creates a stock record linked to an eligible donor.
- Patient blood requests and fulfilment with stock sufficiency checking.
- Blood group validation and ISO date-based expiry checks.
- Summary report, file save/load, input validation, and exception handling.
- Dynamic arrays, constructors/destructors, inheritance and runtime polymorphism.

## Data files
The program saves plain-text pipe-separated records in `Data/`:
- `donors.txt`
- `blood_units.txt`
- `patients.txt`
- `requests.txt`
- `ids.txt`

The application attempts to load records at startup and saves on explicit save and exit. Keep the program running from the project root so relative paths resolve correctly.

## Important limitations
This is an academic demonstration, not a real clinical system. It does not provide authenticated roles, medical compatibility rules, lab screening, privacy controls, or a production database. The blood-group match is exact-match only and should not be used for actual medical decisions.

## Submission checklist
1. Compile and run the program on your own computer.
2. Execute the 15 test cases in `TEST_CASES.md` and fill in actual results after verifying.
3. Capture your own console screenshots and put them in `screenshots/`.
4. Check your name, date, compiler/IDE and executable details in the templates.
5. Submit the ZIP only after reviewing all files and being able to explain the code.
