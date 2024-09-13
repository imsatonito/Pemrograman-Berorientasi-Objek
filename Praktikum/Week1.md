# Tugas Praktikum 1
1. Buatlah table minimall 5 coloumn  dan form minimal 5 input beserta dengan style css nya

## Jawab
```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tabel dan Form Menarik</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 20px;
            background-color: #f0f4f8;
        }
        h2 {
            color: #2c3e50;
            text-align: center;
            margin-bottom: 20px;
        }
        table {
            border-collapse: separate;
            border-spacing: 0;
            width: 100%;
            margin-bottom: 30px;
            background-color: white;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
            overflow: hidden;
        }
        th, td {
            padding: 15px;
            text-align: left;
            border-bottom: 1px solid #e0e0e0;
        }
        th {
            background-color: #3498db;
            color: white;
            font-weight: bold;
            text-transform: uppercase;
        }
        tr:hover {
            background-color: #f5f5f5;
        }
        form {
            max-width: 500px;
            margin: 0 auto;
            background-color: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        label {
            display: block;
            margin-top: 15px;
            color: #2c3e50;
            font-weight: bold;
        }
        input[type="text"], input[type="email"], input[type="tel"], select {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            margin-bottom: 15px;
            border: 1px solid #bdc3c7;
            border-radius: 4px;
            font-size: 16px;
        }
        input[type="submit"] {
            background-color: #2ecc71;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
            font-weight: bold;
            transition: background-color 0.3s ease;
        }
        input[type="submit"]:hover {
            background-color: #27ae60;
        }
    </style>
</head>
<body>
    <h2>Tabel Data Mahasiswa</h2>
    <table>
        <tr>
            <th>No.</th>
            <th>Nama</th>
            <th>NIM</th>
            <th>Jurusan</th>
            <th>Angkatan</th>
        </tr>
        <tr>
            <td>1</td>
            <td>Budi Santoso</td>
            <td>11231001</td>
            <td>Informatika</td>
            <td>2023</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Imam ghozali</td>
            <td>10231012</td>
            <td>Sistem Informasi</td>
            <td>2023</td>
        </tr>
        <tr>
            <td>3</td>
            <td>Ahmad Hidayat</td>
            <td>10231003</td>
            <td>Sistem Informasi</td>
            <td>2023</td>
        </tr>
    </table>

    <h2>Form Pendaftaran Mahasiswa Baru</h2>
    <form>
        <label for="nama">Nama Lengkap:</label>
        <input type="text" id="nama" name="nama" required>

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>

        <label for="telepon">Nomor Telepon:</label>
        <input type="tel" id="telepon" name="telepon" required>

        <label for="jurusan">Jurusan:</label>
        <select id="jurusan" name="jurusan" required>
            <option value="">Pilih Jurusan</option>
            <option value="ti">Informatika</option>
            <option value="si">Sistem Informasi</option>
        </select>

        <label for="alamat">Alamat:</label>
        <input type="text" id="alamat" name="alamat" required>

        <input type="submit" value="Daftar">
    </form>
</body>
</html>

```
