# Given two arrays a and b write a function comp(a, b) that checks whether the two arrays have the "same" elements, 
#  with the same multiplicities. "Same" means, here, that the elements in b are the elements in a squared.

def comp(array1, array2):
    if array1 == None:
        return False
    if array2 == None:
        return False

    square_array = list()
    for item in array1:
        number = item ** 2
        square_array.append(number)
    square_array.sort()
    array2.sort()

    if square_array == array2:
        return True
    else:
        return False

# -----

# Given a string, detect whether or not it is a pangram. Return True if it is, False if not.

def is_pangram(s):
    alphabet = {"a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t", "u", "v",
                "w", "x", "y", "z"}
    lowercase = s.casefold()
    new = set(lowercase)
    return(alphabet.issubset(new))

# -----

# Complete the solution so that the function will break up camel casing, using a space between words.
# "camelCasing"  =>  "camel Casing"

def solution(s):
    answer = list()
    for item in s:
        if item.isupper():
            answer.append(" ")
        answer.append(item)
    final_answer = ''.join(answer)
    return(final_answer)

# -----

# You are going to be given an array of integers. Your job is to take that array and find an index N
# where the sum of the integers to the left of N is equal to the sum of the integers to the right of N.
# If there is no index that would make this happen, return -1.

def find_even_index(arr):
    for idx, item in enumerate(arr):
        left = sum(arr[:idx])
        right = sum(arr[idx + 1:])
        if left == right:
            return (idx)

    return -1

# -----

# Given a positive integer n written as abcd... (a, b, c, d... being digits) and a positive integer p
#we want to find a positive integer k, if it exists, such that the sum of the digits of n taken to the successive
# powers of p is equal to k * n. If it is the case we will return k, if not return -1.

def dig_pow(n, p):
    n_split = list(str(n))
    y = 0
    for item in n_split:
        a = int(item) ** p
        y = y + a
        p = p + 1
    k = y / n
    if y % n == 0:
        return(int(k))
    else:
        return(-1)

# -----

# Your task is to make a function that can take any non-negative integer as an argument and return it with
# its digits in descending order. Essentially, rearrange the digits to create the highest possible number.

def descending_order(num):
    number_list = list(str((num)))
    number_list.sort(reverse=True)
    num_ordered = ''.join(number_list)
    return(int(num_ordered))

# -----

# Usually when you buy something, you're asked whether your credit card number, phone number or answer to your most
# secret question is still correct. However, since someone could look over your shoulder, you don't want that shown
# on your screen. Instead, we mask it.
#
# Your task is to write a function maskify, which changes all but the last four characters into '#'.

def maskify(cc):
    length = len(cc)
    dashes = (length - 4) * "#"
    ending = cc[-4:]

    return(dashes + ending)

# -----
