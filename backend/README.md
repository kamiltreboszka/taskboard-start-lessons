# backend

Serwer Express, który udostępnia API pod adresem `/api` i serwuje pliki frontendu.

| Plik | Do czego służy |
| --- | --- |
| `server.js` | Start serwera, sesja, podłączenie tras, obsługa błędów |
| `db.js` | Pula połączeń z bazą MySQL (`mysql2`), dane z pliku `.env` |
| `utils.js` | Funkcje pomocnicze: walidacja, zamiana id, odpowiedź 400 |
| `middleware/auth.js` | `requireAuth` – bez zalogowania odpowiedź 401 |
| `routes/auth.js` | Rejestracja, logowanie, wylogowanie, dane zalogowanego |
| `routes/users.js` | Lista użytkowników do przypisywania zadań |
| `routes/boards.js` | Tablice: lista, dodawanie, zmiana, soft delete, zadania tablicy |
| `routes/tasks.js` | Zadania: szczegóły, dodawanie, zmiana, soft delete, filtrowanie |

Uruchomienie: `npm install`, potem `npm start` (szczegóły w głównym README).
