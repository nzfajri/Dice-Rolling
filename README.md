# Dice-Rolling
Program Sederhana
#include <iostream>
#include <cstdlib>
#include <ctime>

int main() {
    srand(time(0));

    std::cout <<"Welcome to Dice Rolling "<< std::endl;

    while (true) {
        std::cout << "Gulirkan dadu (y/n)? ";
        char jawaban;
        std::cin >> jawaban;

        if (jawaban == 'n')
            break;

        if (jawaban == 'y') {
            int angka = rand() % 6 + 1;
            std::cout << "Angka dadu: " << angka << std::endl;
        } else {
            std::cout << "Masukkan jawaban yang valid (y/n)!" << std::endl;
        }
    }

    return 0;
}
