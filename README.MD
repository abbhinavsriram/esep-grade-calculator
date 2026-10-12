# ESEP Grade Calculator

This library is a simple utility to calculate your grades.

Three grade types
* assignments (weighted 50%)
* exams (weighted 35%)
* essays (weighted 15%)

Grades are calculated in the following manner:
* Letter cutoffs: A ≥ 90, B ≥ 80, C ≥ 70, D ≥ 60, else F
* Averages are computed per grade type then weighted before summing to create final grade average
* grade type averages and final grades are truncated (no rounding up)


Runtime requirements:
Golang 1.24+

Run unit tests:
```
cd grade-calculator/
go test ./...
```

Run unit tests with code coverage:
```
cd grade-calculator/
go test -coverprofile=coverage.txt ./...
```