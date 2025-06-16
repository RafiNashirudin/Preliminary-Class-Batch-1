# 1. Algorithms & Flowcharts
a. Simbol flowchart

b. pseudocode
```pseudocode
Start

Input n

If n <= 1 then
    Output "Bukan bilangan prima"
    Stop
End If

Set isPrime = true

For i from 2 to √n do
    If n mod i == 0 then
        Set isPrime = false
        Break
    End If
End For

If isPrime == true then
    Output "Bilangan prima"
Else
    Output "Bukan bilangan prima"
End If

Stop
```

# 2. JavaScript: Variabel & Scope
```javascript
let a = 3;
const b = 5;
{
  let a = 10;
  var c = a + b;
}

console.log(a); // Output: 3
console.log(c); // Output: 15
```

# 3. JavaScript: Array Manipulation

```javascript

function reverseArray(arr) {
  let reversed = [];
  for (let i = arr.length - 1; i >= 0; i--) {
    reversed.push(arr[i]);
  }
  return reversed;
}

// hasil
console.log(reverseArray([1, 2, 3]));

```
# 4. Linux CLI
a. Perintah melihat isi direktori saat ini beserta file tersembunyi:
```bash
ls -a
```

b. Perintah mengubah owner file data.txt menjadi user bootcamp:
```bash
sudo chown bootcamp data.txt
```

# 5. Git Workflow
a. Perintah untuk melihat perubahan yang belum di-commit:
```bash
git status
```

b. Setelah membuat branch *feat/search*, perintah untuk:
```bash
git switch feat/search
```

Push branch ke remote:
```bash
git push -u origin feat/search
```

# 6. SQL: DDL & DML
a. Tambahkan kolom stock (INTEGER)
```sql
ALTER TABLE products ADD COLUMN stock INTEGER;
```

b. Update harga product id=5 menjadi 75000
```sql
UPDATE products SET price = 75000 WHERE id = 5;
```

# 7. SQL: Query
```sql
SELECT city, COUNT(*) AS jumlah_user
FROM users
GROUP BY city
HAVING COUNT(*) > 10;
```

# 8. Data Structures: Stack
```
push() = menambahkan elemen ke atas stack
pop() = menghapus elemen paling atas dari stack
```

Tumpukan piring di rak: Piring terakhir yang ditaruh (push) akan menjadi yang pertama diambil (pop). Ini sesuai dengan prinsip LIFO (Last In, First Out).

# 9. Data Structures: Linked List vs Array
Tidak perlu memindahkan elemen lainnya, hanya mengatur ulang pointer.

# 10. Control Flow
```
0
1
2
3
```

# 11. Error Handling

```javascript
try {
  JSON.parse("invalid json");
} catch (err) {
  console.log("Error:", err.message);
}
```

# 12. Git Conflict
a. Edit isi file.

b. Hapus semua tanda konflik (<<<<<<<, =======, >>>>>>>).

c. Tandai file sudah diselesaikan dengan:
```
git add <nama-file>
```

d. Lanjutkan proses merge
```
git commit
```

# 13. Linux File Permission
Owner bisa: Dapat melihat isi, menambahkan/menghapus file, dan masuk ke folder
Group bisa: Dapat melihat isi folder dan masuk ke dalamnya, tapi tidak bisa mengubah isi folder
Others bisa: Hanya bisa melihat nama folder (jika path-nya diketahui), tapi tidak bisa masuk atau melihat isinya

# 14. Recursion
120

# 15.PostgreSQL Connection
```postgresql
psql -U admin -d bootcamp_db
```

# 16. JavaScript: Arrow Function

```javascript
const multiply = (a, b) => a * b;
```

# 17. Tree Traversal
Root → Left → Right

# 18. Package Management
```bash
npm install lodash
```

# 19. Git Log
```bash
git log --oneline --graph --all
```

# 20. SQL: JOIN

```sql
LEFT JOIN departments d ON e.department_id = d.id;
```
