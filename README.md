# welcome to repo 
hello world
```python
import math

def hitung_sisi_miring(a: float, b: float) -> float:
    return math.sqrt(a**2 + b**2)

def hitung_sisi_siku(c: float, sisi_lain: float) -> float:
    return math.sqrt(c**2 - sisi_lain**2)

print("Pilih perhitungan:")
print("1. Hitung sisi miring (c)")
print("2. Hitung sisi siku-siku (a atau b)")

pilihan = input("Masukkan pilihan (1/2): ")

if pilihan == "1":
    a = float(input("Masukkan sisi a: "))
    b = float(input("Masukkan sisi b: "))
    c = hitung_sisi_miring(a, b)
    print(f"Sisi miring (c) = {c:.2f}")

elif pilihan == "2":
    c = float(input("Masukkan sisi miring (c): "))
    sisi_lain = float(input("Masukkan sisi siku lainnya: "))
    sisi_siku = hitung_sisi_siku(c, sisi_lain)
    print(f"Sisi siku yang dicari = {sisi_siku:.2f}")

else:
    print("Pilihan tidak valid.")
```

