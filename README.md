# Group-Work-11.29.2021

    #include <iostream>
    #include <array>
    #include <algorithm>
    using namespace std;
    void arraylibclass() {

    double ave = 0;

    array<int, 20> graderes = {};
    cout << "Please input the marks of 20 students, ranging from 0 to 100" << endl;

    for(int i = 0; i < 20; i++){
        cin >> graderes[i];
        ave += graderes[i];
    }
    sort(graderes.begin(), graderes.end());
    cout << "Ascending order: " << endl;
    for (int numx : graderes){
        cout << numx << " " << endl;
    }
    reverse(graderes.begin(), graderes.end());
    cout << endl;
    cout << "Descending order: " << endl;
    for (int numy : graderes){
    cout << numy << " " << endl;
    }
    cout << endl;
    cout << "Total: " << ave << endl;


    cout << "Class Average: " << ave / graderes.size() << endl;
    cout << "Lowest Grade: " << graderes.at(19) << endl;
    cout << "Highest Grade: " << graderes.at(0) << endl;

    }
    int main(){
    arraylibclass();
    return 0;
    }
