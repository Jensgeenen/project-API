# To-Do List API

Dit project is een eenvoudige To-Do List API waarmee gebruikers taken kunnen beheren. Gebruikers kunnen taken aanmaken, bijwerken, verwijderen, en ophalen. Taken kunnen worden gekoppeld aan projecten en gebruikers. De API is gebouwd met Flask en gebruikt SQLite als database.

## Entiteiten
- **User**: Gebruikers die taken en projecten kunnen beheren.
- **Task**: Taken die door gebruikers kunnen worden aangemaakt en gekoppeld aan projecten.
- **Project**: Projecten waaraan taken gekoppeld kunnen worden.

## API Endpoints

### GET /tasks
Haalt alle taken op.

### GET /tasks/<int:id>
Haalt een specifieke taak op basis van ID.

### POST /tasks
Maakt een nieuwe taak aan. Vereiste velden:
- `title`: De titel van de taak.
- `description`: Een optionele beschrijving van de taak.
- `due_date`: De vervaldatum van de taak (YYYY-MM-DD).
- `user_id`: De ID van de gebruiker die de taak aanmaakt.
- `project_id`: De ID van het project waaraan de taak is gekoppeld.

### PUT /tasks/<int:id>
Werkt een bestaande taak bij.

### DELETE /tasks/<int:id>
Verwijdert een specifieke taak.
### Aantoonbare werking

Hieronder zijn de screenshots toegevoegd van de Postman requests:

- **GET /projects**: ![Get Projects](./Schermafbeelding2024-08-15-224036.png)
- **GET /projects/1**: ![Get Project 1](./Schermafbeelding2024-08-15-224100.png)
- **POST /tasks**: ![Post Task](./Schermafbeelding2024-08-15-224139.png)
- **GET /tasks/1**: ![Get Task 1](./Schermafbeelding2024-08-15-224243.png)
- **PUT /tasks/1**: ![Put Task](./Schermafbeelding2024-08-15-224314.png)
- **GET /tasks**: ![Get Tasks](./Schermafbeelding2024-08-15-224413.png)
- **POST /users**: ![Post User](./Schermafbeelding2024-08-15-223310.png)
- **POST /projects**: ![Post Project](./Schermafbeelding2024-08-15-223358.png)
