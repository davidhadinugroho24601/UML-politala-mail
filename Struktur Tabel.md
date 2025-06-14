Berikut adalah **struktur tabel database dalam format Markdown** sesuai dengan ERD yang kamu berikan:

---

### `users`

| Kolom        | Tipe Data |
| ------------ | --------- |
| id           | bigint    |
| name         | string    |
| email        | string    |
| password     | string    |
| category\_id | int       |

---

### `user_categories`

| Kolom | Tipe Data |
| ----- | --------- |
| id    | bigint    |
| name  | string    |

---

### `groups`

| Kolom        | Tipe Data |
| ------------ | --------- |
| id           | bigint    |
| name         | string    |
| description  | text      |
| parent\_id   | int       |
| manager\_id  | int       |
| acronym      | string    |
| division\_id | int       |

---

### `group_details`

| Kolom     | Tipe Data |
| --------- | --------- |
| id        | bigint    |
| user\_id  | bigint    |
| group\_id | bigint    |

---

### `divisions`

| Kolom          | Tipe Data |
| -------------- | --------- |
| id             | bigint    |
| name           | string    |
| acronym        | string    |
| division\_code | string    |

---

### `dispositions`

| Kolom | Tipe Data |
| ----- | --------- |
| id    | bigint    |
| name  | string    |

---

### `approval_chains`

| Kolom     | Tipe Data |
| --------- | --------- |
| id        | bigint    |
| mail\_id  | bigint    |
| group\_id | bigint    |
| notes     | string    |
| status    | string    |

---

### `attachments`

| Kolom       | Tipe Data |
| ----------- | --------- |
| id          | bigint    |
| description | string    |
| path        | text      |
| mail\_id    | bigint    |

---

### `code_lists`

| Kolom    | Tipe Data |
| -------- | --------- |
| id       | bigint    |
| mail\_id | bigint    |
| code     | string    |

---

### `mails`

| Kolom             | Tipe Data |
| ----------------- | --------- |
| id                | bigint    |
| writer\_id        | bigint    |
| target\_id        | bigint    |
| template\_id      | bigint    |
| final\_id         | bigint    |
| group\_id         | bigint    |
| content           | text      |
| status            | string    |
| is\_staged        | boolean   |
| subject           | string    |
| notes             | text      |
| disposition\_id   | bigint    |
| google\_doc\_link | string    |
| pdf\_path         | string    |
| direct\_id        | bigint    |
| hidden\_code      | string    |
| released          | boolean   |

---

### `mail_codes`

| Kolom        | Tipe Data |
| ------------ | --------- |
| id           | bigint    |
| code\_name   | string    |
| status       | string    |
| section\_qty | int       |
| code         | string    |

---

### `mail_code_details`

| Kolom    | Tipe Data |
| -------- | --------- |
| id       | bigint    |
| text     | string    |
| number   | int       |
| type     | string    |
| code\_id | bigint    |

---

### `mail_paths`

| Kolom        | Tipe Data |
| ------------ | --------- |
| id           | bigint    |
| sender\_id   | bigint    |
| receiver\_id | bigint    |

---

### `path_details`

| Kolom     | Tipe Data |
| --------- | --------- |
| id        | bigint    |
| path\_id  | bigint    |
| group\_id | bigint    |
| order     | int       |

---

### `mail_templates`

| Kolom             | Tipe Data |
| ----------------- | --------- |
| id                | bigint    |
| template          | string    |
| type              | string    |
| name              | string    |
| google\_doc\_link | string    |

---

### `template_availabilities`

| Kolom        | Tipe Data |
| ------------ | --------- |
| id           | bigint    |
| template\_id | bigint    |
| division\_id | bigint    |

---

### `template_permits`

| Kolom        | Tipe Data |
| ------------ | --------- |
| id           | bigint    |
| template\_id | bigint    |
| group\_id    | bigint    |

---

Jika kamu butuh juga daftar relasi antartabel atau foreign key dalam format Markdown, saya bisa bantu buatkan juga.
