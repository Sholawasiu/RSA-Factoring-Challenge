import sys

def find_factors(n):
    """Find a pair of factors for the given number n."""
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return i, n // i
    return n, 1  # Fallback to n and 1 if no factors found

def process_file(filename):
    """Read numbers from the file and print their factorization."""
    with open(filename, 'r') as file:
        for line in file:
            number = int(line.strip())
            p, q = find_factors(number)
            print(f"{number}={p}*{q}")

if __name__ == "__main__":
    if len(sys.argv) != 2:
        print("Usage: factors <file>")
        sys.exit(1)
    
    filename = sys.argv[1]
    process_file(filename)

