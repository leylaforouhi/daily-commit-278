
def is_anagram(first, second):
    normalize = lambda text: sorted(
        char.lower() for char in text if char.isalnum()
    )

    return normalize(first) == normalize(second)


if __name__ == "__main__":
    first = "listen"
    second = "silent"

    print("First:", first)
    print("Second:", second)
    print("Is anagram:", is_anagram(first, second))
