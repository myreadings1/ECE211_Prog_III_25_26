###

Basic Bit Manipulation:

    Check if a number is even or odd: 

C

    int isEven(int num) {
        return !(num & 1); // If the least significant bit is 0, it's even.
    }

    Get the nth bit of a number: 

C

    int getBit(int num, int n) {
        return (num >> n) & 1; // Shift right by n, then AND with 1.
    }

    Set the nth bit of a number: 

C

    int setBit(int num, int n) {
        return num | (1 << n); // OR with a mask where only the nth bit is 1.
    }

    Clear the nth bit of a number: 

C

    int clearBit(int num, int n) {
        return num & ~(1 << n); // AND with a mask where only the nth bit is 0.
    }

    Toggle the nth bit of a number: 

C

    int toggleBit(int num, int n) {
        return num ^ (1 << n); // XOR with a mask where only the nth bit is 1.
    }

Intermediate Problems:

    Swap two numbers without using a temporary variable: 

C

    void swap(int *a, int *b) {
        *a = *a ^ *b;
        *b = *a ^ *b;
        *a = *a ^ *b;
    }

    Count set bits (number of 1s) in an integer: 

C

    int countSetBits(int num) {
        int count = 0;
        while (num > 0) {
            num &= (num - 1); // Brian Kernighan's algorithm
            count++;
        }
        return count;
    }

Reverse bits of an integer.
C

    unsigned int reverseBits(unsigned int num) {
        unsigned int reversed_num = 0;
        int num_bits = sizeof(num) * 8; // Number of bits in the integer
        for (int i = 0; i < num_bits; i++) {
            if ((num >> i) & 1) { // If the i-th bit is set
                reversed_num |= (1 << (num_bits - 1 - i)); // Set the corresponding bit in reversed_num
            }
        }
        return reversed_num;
    }

    Check if a number is a power of 2: 

C

    int isPowerOfTwo(int num) {
        return (num > 0) && ((num & (num - 1)) == 0);
    }
