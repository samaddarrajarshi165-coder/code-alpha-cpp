# code-alpha-cpp
#include <iostream>
#include <iomanip> // for setprecision
using namespace std;

int main() {
    int numCourses;
    cout << "Enter the number of courses: ";
    cin >> numCourses;

    double grades[100], credits[100]; // arrays to store course data
    double totalGradePoints = 0, totalCredits = 0;

    // Input for each course
    for (int i = 0; i < numCourses; i++) {
        cout << "\nCourse " << i + 1 << ":\n";
        cout << "Enter grade (e.g., 8.5): ";
        cin >> grades[i];
        cout << "Enter credit hours: ";
        cin >> credits[i];

        totalGradePoints += grades[i] * credits[i];
        totalCredits += credits[i];
    }

    // Calculate semester GPA
    double semesterGPA = totalGradePoints / totalCredits;

    // Get previous CGPA info
    double prevCGPA, prevTotalCredits;
    cout << "\nEnter previous CGPA: ";
    cin >> prevCGPA;
    cout << "Enter previous total credits: ";
    cin >> prevTotalCredits;

    // Calculate overall CGPA
    double overallCGPA = ((prevCGPA * prevTotalCredits) + (semesterGPA * totalCredits)) 
                         / (prevTotalCredits + totalCredits);

    // Output results
    cout << fixed << setprecision(2); // show 2 decimal places
    cout << "\n--- Course Details ---\n";
    for (int i = 0; i < numCourses; i++) {
        cout << "Course " << i + 1 << ": Grade = " << grades[i]
             << ", Credits = " << credits[i] << endl;
    }

    cout << "\nSemester GPA: " << semesterGPA << endl;
    cout << "Overall CGPA: " << overallCGPA << endl;

    return 0;
}
