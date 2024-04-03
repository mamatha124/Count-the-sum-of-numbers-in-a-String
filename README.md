# Count-the-sum-of-numbers-in-a-String in python
s = input()
sum = 0
i = 0
while i < len(s):
    if s[i].isdigit():
        j = i
        d = 0
        while j < len(s) and s[j].isdigit():
            d = d * 10 + int(s[j])
            j += 1
            i = j
                sum += d
          else:
                i += 1
        print(sum)

