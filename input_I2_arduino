#include <iostream>
#include <stdlib.h>
#include <time.h>
using namespace std;

void timer(int seconds) {
    int milli_seconds = 1000 * seconds;
    clock_t start_time = clock();
    while (clock() < start_time + milli_seconds);
}

int main() {
    int i; int I2; int loop; string choise; 
    do {
        cout << "\n1.and / 2.exit: "; cin >> choise;
        if (choise == "1" || choise == "and") {
            cout << "\nhow many loops: "; cin >> loop;
            for (i = 0; i < loop; i++) {
                cout << "\nI2: "; cin >> I2;
            }
            if (I2 == 1) {
                do {
                    cout << "\nLED on."; 
                    cout << "\n\nLED stays on till I2 == 0.\n\nI2: "; cin >> I2;
                    if (I2 == 0) {
                        main();
                    }
                } while (I2 == 1);
            } else if (I2 == 0) {
                cout << "\ninvalid input 0.\n";
                main();
            }
        } else if (choise == "2" || choise == "exit") {
            for (i = 4; i < 5; i--) {
                cout << i - 1;
                for (i = 3; i < 4; i--) {
                    timer(1);
                    cout << "\n" << i - 1;
                    for (i = 2; i < 3; i--) {
                        timer(1);
                        cout << "\n" << i - 1;
                        for (i = 1; i < 2; i--) {
                            timer(1);
                            cout << "\n" << i - 1;
                            exit(1);
                        }
                    }
                }
            }
        }
    } while (true);
    return 0;
}
