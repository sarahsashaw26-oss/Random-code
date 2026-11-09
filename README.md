cols, rows = 80, 40
for y in range(rows):
    line = ""
    for x in range(cols):
        c = complex((x - cols/1.5) / (cols/3), (y - rows/2) / (rows/3))
        z = 0
        for _ in range(50):
            z = z*z + c
            if abs(z) > 2:
                break
        line += " " if abs(z) <= 2 else "#"
    print(line)
    cols, rows = 90, 40

for y in range(rows):
    line = ""
    for x in range(cols):
        c = complex((x - cols / 1.5) / (cols / 3.2),
                    (y - rows / 2) / (rows / 3.2))
        z = 0
        for _ in range(60):
            z = z * z + c
            if abs(z) > 2:
                break
        line += " " if abs(z) <= 2 else "#"
    print(line)

  import random
print(random.choice(["my cat", "a cosmic ray", "the compiler", "Mercury retrograde"]) + " " + random.choice(["ate", "deleted", "corrupted", "reinterpreted"]) + " " + random.choice(["my code", "the database", "the config file", "the tests"]))
