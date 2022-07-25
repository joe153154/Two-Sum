def two_sum(arr, target):
    for i in range(len(arr)):
        w = i + 1
        for j in range(len(arr[w:])):
            v = j + w
            z = arr[i] + arr[v]
            if z == target:
                print(f"[{i}, {v}]")

def main():
    arr = [1, 7, 11, 13, 18]
    target = 19
    two_sum(arr, target)

if __name__ == "__main__":
    main()