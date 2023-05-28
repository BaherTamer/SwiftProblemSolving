# Grading Students

``` swift
func gradingStudents(grades: [Int]) -> [Int] {
    grades.map { grade in
        grade >= 38 && ((grade / 5 + 1) * 5 - grade) < 3 ? (grade / 5 + 1) * 5 : grade
    }
}
```
