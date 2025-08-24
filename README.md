# **Metode Konstruktor JavaScript**

📅 **2 April 2025** | ⏱ **Waktu Baca: 1 menit**

---

## 📖 Deskripsi
Metode **konstruktor** dalam JavaScript adalah jenis metode khusus yang digunakan untuk **menginisialisasi dan membuat objek**. Metode ini dipanggil secara otomatis ketika **memori dialokasikan untuk objek tersebut**.

---

## ✅ Hal yang Perlu Diingat
- **Kata kunci `constructor` digunakan untuk mendeklarasikan metode konstruktor.**
- **Sebuah kelas hanya dapat memiliki satu metode konstruktor.**
- **JavaScript memungkinkan kita memanggil konstruktor dari kelas induk menggunakan kata kunci `super`.**

---

## 🖥 Contoh Kode
```javascript
class Person {
  constructor(name) {
    this.name = name;
  }
}

class Student extends Person {
  constructor(name, grade) {
    super(name); // Memanggil constructor dari kelas induk
    this.grade = grade;
  }
}

const student1 = new Student('Andi', 'A');
console.log(student1.name);   // Output: Andi
console.log(student1.grade);  // Output: A
