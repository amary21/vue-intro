## Getting started

Install JSON Server

```
npm install -g json-server
```

Start JSON Server

```bash
json-server --watch db.json
```

## Get Best Products

Request :

- Method : GET
- Endpoint : `/best-products`

Response :

```json
{
  "id": 1,
  "kode": "K-01",
  "nama": "Sate Ayam",
  "harga": 16000,
  "is_ready": true,
  "gambar": "sate-ayam.jpg"
}
```

## Get List Products

Request :

- Method : GET
- Endpoint : `/products`

Response :

```json
{
  "id": 1,
  "kode": "K-01",
  "nama": "Sate Ayam",
  "harga": 16000,
  "is_ready": true,
  "gambar": "sate-ayam.jpg"
}
```

## Search Products

Request :

- Method : GET
- Endpoint : `/products?q={search}`

Response :

```json
{
  "id": 1,
  "kode": "K-01",
  "nama": "Sate Ayam",
  "harga": 16000,
  "is_ready": true,
  "gambar": "sate-ayam.jpg"
}
```

## Detail Products

Request :

- Method : GET
- Endpoint : `/products/{id_product}`

Response :

```json
{
  "id": 1,
  "kode": "K-01",
  "nama": "Sate Ayam",
  "harga": 16000,
  "is_ready": true,
  "gambar": "sate-ayam.jpg"
}
```

## Get Keranjang

Request :

- Method : GET
- Endpoint : `/keranjangs`

Response :

```json
{
  "jumlah_pemesanan": "1",
  "products": {
    "id": 2,
    "kode": "K-02",
    "nama": "Nasi Goreng Telur",
    "harga": 14000,
    "is_ready": true,
    "gambar": "nasi-goreng-telor.jpg"
  },
  "id": 1
}
```
