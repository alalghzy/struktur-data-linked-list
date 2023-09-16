#include <iostream>

class Node {
public:
    int info;
    Node* next;
};

class List {
private:
    Node* first;
    Node* last;

public:
    List() : first(nullptr), last(nullptr) {}

    void Buat();
    void Tambahkan();
    void Hapus();
    void Tampil();
    void Cari();
};

void List::Buat() {
    Node* temp = new Node;
    int n;
    std::cout << "\nInput Elemen:";
    std::cin >> n;
    temp->info = n;
    temp->next = nullptr;
    if (first == nullptr) {
        first = temp;
        last = first;
    } else {
        last->next = temp;
        last = temp;
    }
}

// Implementasi fungsi-fungsi lainnya

int main() {
    List l;
    int ch;
    while (1) {
        std::cout << "\n** MENU **";
        std::cout << "\n1:Buat\n2:Tambahkan\n3:Hapus\n4:Cari\n5:Tampilkan\n6:Keluar Program\n";
        std::cout << "\nInput pilihan anda:";
        std::cin >> ch;
        switch (ch) {
            case 1:
                l.Buat();
                break;
            case 2:
                l.Tambahkan();
                break;
            case 3:
                l.Hapus();
                break;
            case 4:
                l.Cari();
                break;
            case 5:
                l.Tampil();
                break;
            case 6:
                return 0;
        }
    }
    return 0;
}
